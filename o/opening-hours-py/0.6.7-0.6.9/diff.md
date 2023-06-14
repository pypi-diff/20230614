# Comparing `tmp/opening_hours_py-0.6.7.tar.gz` & `tmp/opening_hours_py-0.6.9.tar.gz`

## Comparing `opening_hours_py-0.6.7.tar` & `opening_hours_py-0.6.9.tar`

### file list

```diff
@@ -1,68 +1,68 @@
--rw-r--r--   0        0        0      514 1970-01-01 00:00:00.000000 opening_hours_py-0.6.7/local_dependencies/compact-calendar/Cargo.toml
--rw-r--r--   0     1001      123     1588 2023-06-14 14:01:22.000000 opening_hours_py-0.6.7/local_dependencies/compact-calendar/README.md
--rw-r--r--   0     1001      123    23597 2023-06-14 14:01:22.000000 opening_hours_py-0.6.7/local_dependencies/compact-calendar/src/lib.rs
--rw-r--r--   0        0        0      935 1970-01-01 00:00:00.000000 opening_hours_py-0.6.7/local_dependencies/opening-hours/Cargo.toml
--rw-r--r--   0     1001      123       86 2023-06-14 14:01:22.000000 opening_hours_py-0.6.7/local_dependencies/opening-hours/.github/codecov.yml
--rw-r--r--   0     1001      123     2837 2023-06-14 14:01:22.000000 opening_hours_py-0.6.7/local_dependencies/opening-hours/.github/workflows/deploy.yml
--rw-r--r--   0     1001      123     2325 2023-06-14 14:01:22.000000 opening_hours_py-0.6.7/local_dependencies/opening-hours/.github/workflows/tests.yml
--rw-r--r--   0     1001      123       49 2023-06-14 14:01:22.000000 opening_hours_py-0.6.7/local_dependencies/opening-hours/.gitignore
--rw-r--r--   0     1001      123       22 2023-06-14 14:01:22.000000 opening_hours_py-0.6.7/local_dependencies/opening-hours/.rustfmt.toml
--rw-r--r--   0     1001      123    29444 2023-06-14 14:01:22.000000 opening_hours_py-0.6.7/local_dependencies/opening-hours/Cargo.lock
--rw-r--r--   0     1001      123    10847 2023-06-14 14:01:22.000000 opening_hours_py-0.6.7/local_dependencies/opening-hours/LICENSE-APACHE
--rw-r--r--   0     1001      123     1056 2023-06-14 14:01:22.000000 opening_hours_py-0.6.7/local_dependencies/opening-hours/LICENSE-MIT
--rw-r--r--   0     1001      123     2800 2023-06-14 14:01:22.000000 opening_hours_py-0.6.7/local_dependencies/opening-hours/README.md
--rw-r--r--   0     1001      123     1996 2023-06-14 14:01:22.000000 opening_hours_py-0.6.7/local_dependencies/opening-hours/benches/benchmarks.rs
--rw-r--r--   0     1001      123     2368 2023-06-14 14:01:22.000000 opening_hours_py-0.6.7/local_dependencies/opening-hours/build.rs
--rw-r--r--   0     1001      123  4657878 2023-06-14 14:01:22.000000 opening_hours_py-0.6.7/local_dependencies/opening-hours/data/holidays.txt
--rwxr-xr-x   0     1001      123     3275 2023-06-14 14:01:22.000000 opening_hours_py-0.6.7/local_dependencies/opening-hours/scripts/check-version.py
--rwxr-xr-x   0     1001      123     1092 2023-06-14 14:01:22.000000 opening_hours_py-0.6.7/local_dependencies/opening-hours/scripts/generate-holidays.py
--rw-r--r--   0     1001      123    12546 2023-06-14 14:01:22.000000 opening_hours_py-0.6.7/local_dependencies/opening-hours/scripts/poetry.lock
--rw-r--r--   0     1001      123      428 2023-06-14 14:01:22.000000 opening_hours_py-0.6.7/local_dependencies/opening-hours/scripts/pyproject.toml
--rw-r--r--   0     1001      123     1370 2023-06-14 14:01:22.000000 opening_hours_py-0.6.7/local_dependencies/opening-hours/src/bin/schedule.rs
--rw-r--r--   0     1001      123    12893 2023-06-14 14:01:22.000000 opening_hours_py-0.6.7/local_dependencies/opening-hours/src/date_filter.rs
--rw-r--r--   0     1001      123      400 2023-06-14 14:01:22.000000 opening_hours_py-0.6.7/local_dependencies/opening-hours/src/lib.rs
--rw-r--r--   0     1001      123    11396 2023-06-14 14:01:22.000000 opening_hours_py-0.6.7/local_dependencies/opening-hours/src/opening_hours.rs
--rw-r--r--   0     1001      123     6628 2023-06-14 14:01:22.000000 opening_hours_py-0.6.7/local_dependencies/opening-hours/src/schedule.rs
--rw-r--r--   0     1001      123     9791 2023-06-14 14:01:22.000000 opening_hours_py-0.6.7/local_dependencies/opening-hours/src/tests/data/sample.txt
--rw-r--r--   0     1001      123      824 2023-06-14 14:01:22.000000 opening_hours_py-0.6.7/local_dependencies/opening-hours/src/tests/holiday_selector.rs
--rw-r--r--   0     1001      123      905 2023-06-14 14:01:22.000000 opening_hours_py-0.6.7/local_dependencies/opening-hours/src/tests/issues.rs
--rw-r--r--   0     1001      123     2501 2023-06-14 14:01:22.000000 opening_hours_py-0.6.7/local_dependencies/opening-hours/src/tests/mod.rs
--rw-r--r--   0     1001      123     1487 2023-06-14 14:01:22.000000 opening_hours_py-0.6.7/local_dependencies/opening-hours/src/tests/month_selector.rs
--rw-r--r--   0     1001      123     1528 2023-06-14 14:01:22.000000 opening_hours_py-0.6.7/local_dependencies/opening-hours/src/tests/next_change.rs
--rw-r--r--   0     1001      123      497 2023-06-14 14:01:22.000000 opening_hours_py-0.6.7/local_dependencies/opening-hours/src/tests/next_change_hint.rs
--rw-r--r--   0     1001      123      339 2023-06-14 14:01:22.000000 opening_hours_py-0.6.7/local_dependencies/opening-hours/src/tests/parser.rs
--rw-r--r--   0     1001      123     2790 2023-06-14 14:01:22.000000 opening_hours_py-0.6.7/local_dependencies/opening-hours/src/tests/rules.rs
--rw-r--r--   0     1001      123     3243 2023-06-14 14:01:22.000000 opening_hours_py-0.6.7/local_dependencies/opening-hours/src/tests/selective.rs
--rw-r--r--   0     1001      123     1598 2023-06-14 14:01:22.000000 opening_hours_py-0.6.7/local_dependencies/opening-hours/src/tests/time_selector.rs
--rw-r--r--   0     1001      123     1176 2023-06-14 14:01:22.000000 opening_hours_py-0.6.7/local_dependencies/opening-hours/src/tests/week_selector.rs
--rw-r--r--   0     1001      123     2541 2023-06-14 14:01:22.000000 opening_hours_py-0.6.7/local_dependencies/opening-hours/src/tests/weekday_selector.rs
--rw-r--r--   0     1001      123     1419 2023-06-14 14:01:22.000000 opening_hours_py-0.6.7/local_dependencies/opening-hours/src/tests/year_selector.rs
--rw-r--r--   0     1001      123     3287 2023-06-14 14:01:22.000000 opening_hours_py-0.6.7/local_dependencies/opening-hours/src/time_filter.rs
--rw-r--r--   0     1001      123       22 2023-06-14 14:01:22.000000 opening_hours_py-0.6.7/local_dependencies/opening-hours/src/utils/mod.rs
--rw-r--r--   0     1001      123     3872 2023-06-14 14:01:22.000000 opening_hours_py-0.6.7/local_dependencies/opening-hours/src/utils/range.rs
--rw-r--r--   0        0        0      551 1970-01-01 00:00:00.000000 opening_hours_py-0.6.7/local_dependencies/opening-hours-syntax/Cargo.toml
--rw-r--r--   0     1001      123    10847 2023-06-14 14:01:22.000000 opening_hours_py-0.6.7/local_dependencies/opening-hours-syntax/LICENSE-APACHE
--rw-r--r--   0     1001      123     1056 2023-06-14 14:01:22.000000 opening_hours_py-0.6.7/local_dependencies/opening-hours-syntax/LICENSE-MIT
--rw-r--r--   0     1001      123      874 2023-06-14 14:01:22.000000 opening_hours_py-0.6.7/local_dependencies/opening-hours-syntax/README.md
--rw-r--r--   0     1001      123      859 2023-06-14 14:01:22.000000 opening_hours_py-0.6.7/local_dependencies/opening-hours-syntax/src/error.rs
--rw-r--r--   0     1001      123     2087 2023-06-14 14:01:22.000000 opening_hours_py-0.6.7/local_dependencies/opening-hours-syntax/src/extended_time.rs
--rw-r--r--   0     1001      123     6513 2023-06-14 14:01:22.000000 opening_hours_py-0.6.7/local_dependencies/opening-hours-syntax/src/grammar.pest
--rw-r--r--   0     1001      123      810 2023-06-14 14:01:22.000000 opening_hours_py-0.6.7/local_dependencies/opening-hours-syntax/src/lib.rs
--rw-r--r--   0     1001      123    24312 2023-06-14 14:01:22.000000 opening_hours_py-0.6.7/local_dependencies/opening-hours-syntax/src/parser.rs
--rw-r--r--   0     1001      123     4206 2023-06-14 14:01:22.000000 opening_hours_py-0.6.7/local_dependencies/opening-hours-syntax/src/rules/day.rs
--rw-r--r--   0     1001      123      584 2023-06-14 14:01:22.000000 opening_hours_py-0.6.7/local_dependencies/opening-hours-syntax/src/rules/mod.rs
--rw-r--r--   0     1001      123     1381 2023-06-14 14:01:22.000000 opening_hours_py-0.6.7/local_dependencies/opening-hours-syntax/src/rules/time.rs
--rw-r--r--   0     1001      123     4048 2023-06-14 14:01:22.000000 opening_hours_py-0.6.7/local_dependencies/opening-hours-syntax/src/sorted_vec.rs
--rw-r--r--   0        0        0      824 1970-01-01 00:00:00.000000 opening_hours_py-0.6.7/Cargo.toml
--rw-r--r--   0     1001      123       40 2023-06-14 14:01:22.000000 opening_hours_py-0.6.7/.gitignore
--rw-r--r--   0     1001      123    10847 2023-06-14 14:01:22.000000 opening_hours_py-0.6.7/LICENSE-APACHE
--rw-r--r--   0     1001      123     1056 2023-06-14 14:01:22.000000 opening_hours_py-0.6.7/LICENSE-MIT
--rw-r--r--   0     1001      123     1871 2023-06-14 14:01:22.000000 opening_hours_py-0.6.7/README.md
--rw-r--r--   0     1001      123    14166 2023-06-14 14:01:22.000000 opening_hours_py-0.6.7/poetry.lock
--rw-r--r--   0     1001      123      374 2023-06-14 14:01:22.000000 opening_hours_py-0.6.7/pyproject.toml
--rwxr-xr-x   0     1001      123      490 2023-06-14 14:01:22.000000 opening_hours_py-0.6.7/run_doctests.py
--rw-r--r--   0     1001      123      692 2023-06-14 14:01:22.000000 opening_hours_py-0.6.7/src/errors.rs
--rw-r--r--   0     1001      123     6474 2023-06-14 14:01:22.000000 opening_hours_py-0.6.7/src/lib.rs
--rw-r--r--   0     1001      123     4967 2023-06-14 14:01:22.000000 opening_hours_py-0.6.7/src/types.rs
--rw-r--r--   0     1001      123    29444 2023-06-14 14:01:22.000000 opening_hours_py-0.6.7/Cargo.lock
--rw-r--r--   0        0        0     2344 1970-01-01 00:00:00.000000 opening_hours_py-0.6.7/PKG-INFO
+-rw-r--r--   0        0        0      935 1970-01-01 00:00:00.000000 opening_hours_py-0.6.9/local_dependencies/opening-hours/Cargo.toml
+-rw-r--r--   0     1001      123       86 2023-06-14 14:17:47.000000 opening_hours_py-0.6.9/local_dependencies/opening-hours/.github/codecov.yml
+-rw-r--r--   0     1001      123     2740 2023-06-14 14:17:47.000000 opening_hours_py-0.6.9/local_dependencies/opening-hours/.github/workflows/deploy.yml
+-rw-r--r--   0     1001      123     2325 2023-06-14 14:17:47.000000 opening_hours_py-0.6.9/local_dependencies/opening-hours/.github/workflows/tests.yml
+-rw-r--r--   0     1001      123       49 2023-06-14 14:17:47.000000 opening_hours_py-0.6.9/local_dependencies/opening-hours/.gitignore
+-rw-r--r--   0     1001      123       22 2023-06-14 14:17:47.000000 opening_hours_py-0.6.9/local_dependencies/opening-hours/.rustfmt.toml
+-rw-r--r--   0     1001      123    29712 2023-06-14 14:17:47.000000 opening_hours_py-0.6.9/local_dependencies/opening-hours/Cargo.lock
+-rw-r--r--   0     1001      123    10847 2023-06-14 14:17:47.000000 opening_hours_py-0.6.9/local_dependencies/opening-hours/LICENSE-APACHE
+-rw-r--r--   0     1001      123     1056 2023-06-14 14:17:47.000000 opening_hours_py-0.6.9/local_dependencies/opening-hours/LICENSE-MIT
+-rw-r--r--   0     1001      123     2800 2023-06-14 14:17:47.000000 opening_hours_py-0.6.9/local_dependencies/opening-hours/README.md
+-rw-r--r--   0     1001      123     1996 2023-06-14 14:17:47.000000 opening_hours_py-0.6.9/local_dependencies/opening-hours/benches/benchmarks.rs
+-rw-r--r--   0     1001      123     2368 2023-06-14 14:17:47.000000 opening_hours_py-0.6.9/local_dependencies/opening-hours/build.rs
+-rw-r--r--   0     1001      123  4657878 2023-06-14 14:17:47.000000 opening_hours_py-0.6.9/local_dependencies/opening-hours/data/holidays.txt
+-rwxr-xr-x   0     1001      123     3275 2023-06-14 14:17:47.000000 opening_hours_py-0.6.9/local_dependencies/opening-hours/scripts/check-version.py
+-rwxr-xr-x   0     1001      123     1092 2023-06-14 14:17:47.000000 opening_hours_py-0.6.9/local_dependencies/opening-hours/scripts/generate-holidays.py
+-rw-r--r--   0     1001      123    12546 2023-06-14 14:17:47.000000 opening_hours_py-0.6.9/local_dependencies/opening-hours/scripts/poetry.lock
+-rw-r--r--   0     1001      123      428 2023-06-14 14:17:47.000000 opening_hours_py-0.6.9/local_dependencies/opening-hours/scripts/pyproject.toml
+-rw-r--r--   0     1001      123     1370 2023-06-14 14:17:47.000000 opening_hours_py-0.6.9/local_dependencies/opening-hours/src/bin/schedule.rs
+-rw-r--r--   0     1001      123    12893 2023-06-14 14:17:47.000000 opening_hours_py-0.6.9/local_dependencies/opening-hours/src/date_filter.rs
+-rw-r--r--   0     1001      123      400 2023-06-14 14:17:47.000000 opening_hours_py-0.6.9/local_dependencies/opening-hours/src/lib.rs
+-rw-r--r--   0     1001      123    11396 2023-06-14 14:17:47.000000 opening_hours_py-0.6.9/local_dependencies/opening-hours/src/opening_hours.rs
+-rw-r--r--   0     1001      123     6628 2023-06-14 14:17:47.000000 opening_hours_py-0.6.9/local_dependencies/opening-hours/src/schedule.rs
+-rw-r--r--   0     1001      123     9791 2023-06-14 14:17:47.000000 opening_hours_py-0.6.9/local_dependencies/opening-hours/src/tests/data/sample.txt
+-rw-r--r--   0     1001      123      824 2023-06-14 14:17:47.000000 opening_hours_py-0.6.9/local_dependencies/opening-hours/src/tests/holiday_selector.rs
+-rw-r--r--   0     1001      123      905 2023-06-14 14:17:47.000000 opening_hours_py-0.6.9/local_dependencies/opening-hours/src/tests/issues.rs
+-rw-r--r--   0     1001      123     2501 2023-06-14 14:17:47.000000 opening_hours_py-0.6.9/local_dependencies/opening-hours/src/tests/mod.rs
+-rw-r--r--   0     1001      123     1487 2023-06-14 14:17:47.000000 opening_hours_py-0.6.9/local_dependencies/opening-hours/src/tests/month_selector.rs
+-rw-r--r--   0     1001      123     1528 2023-06-14 14:17:47.000000 opening_hours_py-0.6.9/local_dependencies/opening-hours/src/tests/next_change.rs
+-rw-r--r--   0     1001      123      497 2023-06-14 14:17:47.000000 opening_hours_py-0.6.9/local_dependencies/opening-hours/src/tests/next_change_hint.rs
+-rw-r--r--   0     1001      123      339 2023-06-14 14:17:47.000000 opening_hours_py-0.6.9/local_dependencies/opening-hours/src/tests/parser.rs
+-rw-r--r--   0     1001      123     2790 2023-06-14 14:17:47.000000 opening_hours_py-0.6.9/local_dependencies/opening-hours/src/tests/rules.rs
+-rw-r--r--   0     1001      123     3243 2023-06-14 14:17:47.000000 opening_hours_py-0.6.9/local_dependencies/opening-hours/src/tests/selective.rs
+-rw-r--r--   0     1001      123     1598 2023-06-14 14:17:47.000000 opening_hours_py-0.6.9/local_dependencies/opening-hours/src/tests/time_selector.rs
+-rw-r--r--   0     1001      123     1176 2023-06-14 14:17:47.000000 opening_hours_py-0.6.9/local_dependencies/opening-hours/src/tests/week_selector.rs
+-rw-r--r--   0     1001      123     2541 2023-06-14 14:17:47.000000 opening_hours_py-0.6.9/local_dependencies/opening-hours/src/tests/weekday_selector.rs
+-rw-r--r--   0     1001      123     1419 2023-06-14 14:17:47.000000 opening_hours_py-0.6.9/local_dependencies/opening-hours/src/tests/year_selector.rs
+-rw-r--r--   0     1001      123     3287 2023-06-14 14:17:47.000000 opening_hours_py-0.6.9/local_dependencies/opening-hours/src/time_filter.rs
+-rw-r--r--   0     1001      123       22 2023-06-14 14:17:47.000000 opening_hours_py-0.6.9/local_dependencies/opening-hours/src/utils/mod.rs
+-rw-r--r--   0     1001      123     3872 2023-06-14 14:17:47.000000 opening_hours_py-0.6.9/local_dependencies/opening-hours/src/utils/range.rs
+-rw-r--r--   0        0        0      514 1970-01-01 00:00:00.000000 opening_hours_py-0.6.9/local_dependencies/compact-calendar/Cargo.toml
+-rw-r--r--   0     1001      123     1588 2023-06-14 14:17:47.000000 opening_hours_py-0.6.9/local_dependencies/compact-calendar/README.md
+-rw-r--r--   0     1001      123    23597 2023-06-14 14:17:47.000000 opening_hours_py-0.6.9/local_dependencies/compact-calendar/src/lib.rs
+-rw-r--r--   0        0        0      551 1970-01-01 00:00:00.000000 opening_hours_py-0.6.9/local_dependencies/opening-hours-syntax/Cargo.toml
+-rw-r--r--   0     1001      123    10847 2023-06-14 14:17:47.000000 opening_hours_py-0.6.9/local_dependencies/opening-hours-syntax/LICENSE-APACHE
+-rw-r--r--   0     1001      123     1056 2023-06-14 14:17:47.000000 opening_hours_py-0.6.9/local_dependencies/opening-hours-syntax/LICENSE-MIT
+-rw-r--r--   0     1001      123      874 2023-06-14 14:17:47.000000 opening_hours_py-0.6.9/local_dependencies/opening-hours-syntax/README.md
+-rw-r--r--   0     1001      123      859 2023-06-14 14:17:47.000000 opening_hours_py-0.6.9/local_dependencies/opening-hours-syntax/src/error.rs
+-rw-r--r--   0     1001      123     2087 2023-06-14 14:17:47.000000 opening_hours_py-0.6.9/local_dependencies/opening-hours-syntax/src/extended_time.rs
+-rw-r--r--   0     1001      123     6513 2023-06-14 14:17:47.000000 opening_hours_py-0.6.9/local_dependencies/opening-hours-syntax/src/grammar.pest
+-rw-r--r--   0     1001      123      810 2023-06-14 14:17:47.000000 opening_hours_py-0.6.9/local_dependencies/opening-hours-syntax/src/lib.rs
+-rw-r--r--   0     1001      123    24312 2023-06-14 14:17:47.000000 opening_hours_py-0.6.9/local_dependencies/opening-hours-syntax/src/parser.rs
+-rw-r--r--   0     1001      123     4206 2023-06-14 14:17:47.000000 opening_hours_py-0.6.9/local_dependencies/opening-hours-syntax/src/rules/day.rs
+-rw-r--r--   0     1001      123      584 2023-06-14 14:17:47.000000 opening_hours_py-0.6.9/local_dependencies/opening-hours-syntax/src/rules/mod.rs
+-rw-r--r--   0     1001      123     1381 2023-06-14 14:17:47.000000 opening_hours_py-0.6.9/local_dependencies/opening-hours-syntax/src/rules/time.rs
+-rw-r--r--   0     1001      123     4048 2023-06-14 14:17:47.000000 opening_hours_py-0.6.9/local_dependencies/opening-hours-syntax/src/sorted_vec.rs
+-rw-r--r--   0        0        0      824 1970-01-01 00:00:00.000000 opening_hours_py-0.6.9/Cargo.toml
+-rw-r--r--   0     1001      123       40 2023-06-14 14:17:47.000000 opening_hours_py-0.6.9/.gitignore
+-rw-r--r--   0     1001      123    10847 2023-06-14 14:17:47.000000 opening_hours_py-0.6.9/LICENSE-APACHE
+-rw-r--r--   0     1001      123     1056 2023-06-14 14:17:47.000000 opening_hours_py-0.6.9/LICENSE-MIT
+-rw-r--r--   0     1001      123     1871 2023-06-14 14:17:47.000000 opening_hours_py-0.6.9/README.md
+-rw-r--r--   0     1001      123    12755 2023-06-14 14:17:47.000000 opening_hours_py-0.6.9/poetry.lock
+-rw-r--r--   0     1001      123      374 2023-06-14 14:17:47.000000 opening_hours_py-0.6.9/pyproject.toml
+-rwxr-xr-x   0     1001      123      490 2023-06-14 14:17:47.000000 opening_hours_py-0.6.9/run_doctests.py
+-rw-r--r--   0     1001      123      692 2023-06-14 14:17:47.000000 opening_hours_py-0.6.9/src/errors.rs
+-rw-r--r--   0     1001      123     6474 2023-06-14 14:17:47.000000 opening_hours_py-0.6.9/src/lib.rs
+-rw-r--r--   0     1001      123     4967 2023-06-14 14:17:47.000000 opening_hours_py-0.6.9/src/types.rs
+-rw-r--r--   0     1001      123    29712 2023-06-14 14:17:47.000000 opening_hours_py-0.6.9/Cargo.lock
+-rw-r--r--   0        0        0     2344 1970-01-01 00:00:00.000000 opening_hours_py-0.6.9/PKG-INFO
```

### Comparing `opening_hours_py-0.6.7/local_dependencies/compact-calendar/Cargo.toml` & `opening_hours_py-0.6.9/local_dependencies/compact-calendar/Cargo.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "compact-calendar"
-version = "0.6.7"
+version = "0.6.9"
 authors = ["Rémi Dupré <remi@dupre.io>"]
 license = "MIT OR Apache-2.0"
 readme = "README.md"
 repository = "https://github.com/remi-dupre/opening-hours-rs"
 documentation = "https://docs.rs/compact-calendar"
 homepage = "https://github.com/remi-dupre/opening-hours-rs/tree/master/compact-calendar"
 description = "Compact representation of a set of days based on a bit-maps"
```

### Comparing `opening_hours_py-0.6.7/local_dependencies/compact-calendar/README.md` & `opening_hours_py-0.6.9/local_dependencies/compact-calendar/README.md`

 * *Files identical despite different names*

### Comparing `opening_hours_py-0.6.7/local_dependencies/compact-calendar/src/lib.rs` & `opening_hours_py-0.6.9/local_dependencies/compact-calendar/src/lib.rs`

 * *Files identical despite different names*

### Comparing `opening_hours_py-0.6.7/local_dependencies/opening-hours/Cargo.toml` & `opening_hours_py-0.6.9/local_dependencies/opening-hours/Cargo.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "opening-hours"
-version = "0.6.7"
+version = "0.6.9"
 authors = ["Rémi Dupré <remi@dupre.io>"]
 license = "MIT OR Apache-2.0"
 readme = "README.md"
 repository = "https://github.com/remi-dupre/opening-hours-rs"
 documentation = "https://docs.rs/opening-hours"
 homepage = "https://github.com/remi-dupre/opening-hours-rs"
 description = "A parser and evaluation tool for the opening_hours fields in OpenStreetMap."
```

### Comparing `opening_hours_py-0.6.7/local_dependencies/opening-hours/.github/workflows/deploy.yml` & `opening_hours_py-0.6.9/local_dependencies/opening-hours/.github/workflows/deploy.yml`

 * *Files 9% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     defaults:
       run:
         working-directory: scripts
 
     steps:
       - uses: actions/checkout@v2
 
-      - uses: actions/setup-python@v2
+      - uses: actions/setup-python@v4
         with:
           python-version: "3.9"
 
       - name: Install poetry
         run: |
           python -m pip install --upgrade pip
           pip install poetry
@@ -77,37 +77,33 @@
   # ---
   # --- Build and deploy Python bindings
   # ---
 
   deploy-python:
     runs-on: ubuntu-latest
 
-    strategy:
-      matrix:
-        python:
-          - "3.9"
-          - "3.10"
-          - "3.11"
-
     defaults:
       run:
         working-directory: python
 
     steps:
       - uses: actions/checkout@v2
 
       - uses: actions-rs/toolchain@v1
         with:
           toolchain: stable
           default: true
           profile: minimal
 
-      - uses: actions/setup-python@v2
+      - uses: actions/setup-python@v4
         with:
-          python-version: ${{ matrix.python }}
+          python-version: |
+            3.9
+            3.10
+            3.11
 
       - name: Install poetry
         run: |
           python -m pip install --upgrade pip
           pip install poetry
 
       - name: Install dependancies
@@ -124,11 +120,11 @@
         if: github.ref == 'refs/heads/master'
         env:
           USER: remi-dupre
           PASS: ${{ secrets.PYPI_PASSWORD }}
 
       - name: Publish to github pages
         uses: peaceiris/actions-gh-pages@v3
-        if: github.ref == 'refs/heads/master' && matrix.python == '3.11'
+        if: github.ref == 'refs/heads/master'
         with:
           github_token: ${{ secrets.GITHUB_TOKEN }}
           publish_dir: ./python/docs
```

### Comparing `opening_hours_py-0.6.7/local_dependencies/opening-hours/.github/workflows/tests.yml` & `opening_hours_py-0.6.9/local_dependencies/opening-hours/.github/workflows/tests.yml`

 * *Files 4% similar despite different names*

```diff
@@ -65,15 +65,15 @@
 
       - uses: actions-rs/toolchain@v1
         with:
           toolchain: stable
           default: true
           profile: minimal
 
-      - uses: actions/setup-python@v2
+      - uses: actions/setup-python@v4
         with:
           python-version: "3.9"
 
       - name: Install poetry
         run: |
           python -m pip install --upgrade pip
           pip install poetry
```

### Comparing `opening_hours_py-0.6.7/local_dependencies/opening-hours/Cargo.lock` & `opening_hours_py-0.6.9/local_dependencies/opening-hours/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -33,17 +33,17 @@
 name = "anstyle"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "41ed9a86bf92ae6580e0a31281f65a1b1d867c0cc68d5346e2ae128dddfa6a7d"
 
 [[package]]
 name = "arbitrary"
-version = "0.4.7"
+version = "1.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "db55d72333851e17d572bec876e390cd3b11eb1ef53ae821dd9f3b653d2b4569"
+checksum = "e2d098ff73c1ca148721f37baad5ea6a465a13f9573aba8641fbbbae8164a54e"
 dependencies = [
  "derive_arbitrary",
 ]
 
 [[package]]
 name = "autocfg"
 version = "1.1.0"
@@ -78,14 +78,17 @@
 checksum = "37b2a672a2cb129a2e41c10b1224bb368f9f37a2b16b612598138befd7b37eb5"
 
 [[package]]
 name = "cc"
 version = "1.0.79"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "50d30906286121d95be3d479533b458f87493b30a4b5f79a607db8f5d11aa91f"
+dependencies = [
+ "jobserver",
+]
 
 [[package]]
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
@@ -155,15 +158,15 @@
 name = "clap_lex"
 version = "0.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2da6da31387c7e4ef160ffab6d5e7f00c42626fe39aea70a7b0f1773f7dd6c1b"
 
 [[package]]
 name = "compact-calendar"
-version = "0.6.7"
+version = "0.6.9"
 dependencies = [
  "chrono",
 ]
 
 [[package]]
 name = "core-foundation-sys"
 version = "0.8.4"
@@ -275,21 +278,21 @@
 dependencies = [
  "generic-array",
  "typenum",
 ]
 
 [[package]]
 name = "derive_arbitrary"
-version = "0.4.7"
+version = "1.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b1a012b5e473dc912f0db0546a1c9c6a194ce8494feb66fa0237160926f9e0e6"
+checksum = "53e0efad4403bfc52dc201159c4b842a246a14b98c64b55dfd0f2d89729dfeb8"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 1.0.109",
+ "syn 2.0.18",
 ]
 
 [[package]]
 name = "digest"
 version = "0.10.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9ed9a281f7bc9b7576e61468ba615a66a5c8cfdff42420a70aa82701a3b1e292"
@@ -440,14 +443,23 @@
 [[package]]
 name = "itoa"
 version = "1.0.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "453ad9f582a441959e5f0d088b02ce04cfe8d51a8eaf077f12ac6d3e94164ca6"
 
 [[package]]
+name = "jobserver"
+version = "0.1.26"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "936cfd212a0155903bcbc060e316fb6cc7cbf2e1907329391ebadc1fe0ce77c2"
+dependencies = [
+ "libc",
+]
+
+[[package]]
 name = "js-sys"
 version = "0.3.64"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c5f195fe497f702db0f318b07fdd68edb16955aed830df8363d837542f8f935a"
 dependencies = [
  "wasm-bindgen",
 ]
@@ -456,20 +468,21 @@
 name = "libc"
 version = "0.2.146"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f92be4933c13fd498862a9e02a3055f8a8d9c039ce33db97306fd5a6caa7f29b"
 
 [[package]]
 name = "libfuzzer-sys"
-version = "0.3.5"
+version = "0.4.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fcf184a4b6b274f82a5df6b357da6055d3e82272327bba281c28bbba6f1664ef"
+checksum = "beb09950ae85a0a94b27676cccf37da5ff13f27076aa1adbc6545dd0d0e1bd4e"
 dependencies = [
  "arbitrary",
  "cc",
+ "once_cell",
 ]
 
 [[package]]
 name = "linux-raw-sys"
 version = "0.3.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ef53942eb7bf7ff43a617b3e2c1c4a5ecf5944a7c1bc12d7ee39bbb15e5c1519"
@@ -537,37 +550,37 @@
 name = "oorandom"
 version = "11.1.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0ab1bc2a289d34bd04a330323ac98a1b4bc82c9d9fcb1e66b63caa84da26b575"
 
 [[package]]
 name = "opening-hours"
-version = "0.6.7"
+version = "0.6.9"
 dependencies = [
  "chrono",
  "compact-calendar",
  "criterion",
  "flate2",
  "once_cell",
  "opening-hours-syntax",
 ]
 
 [[package]]
 name = "opening-hours-py"
-version = "0.6.7"
+version = "0.6.9"
 dependencies = [
  "chrono",
  "opening-hours",
  "opening-hours-syntax",
  "pyo3",
 ]
 
 [[package]]
 name = "opening-hours-syntax"
-version = "0.6.7"
+version = "0.6.9"
 dependencies = [
  "chrono",
  "pest",
  "pest_derive",
 ]
 
 [[package]]
```

### Comparing `opening_hours_py-0.6.7/local_dependencies/opening-hours/LICENSE-APACHE` & `opening_hours_py-0.6.9/local_dependencies/opening-hours/LICENSE-APACHE`

 * *Files identical despite different names*

### Comparing `opening_hours_py-0.6.7/local_dependencies/opening-hours/LICENSE-MIT` & `opening_hours_py-0.6.9/local_dependencies/opening-hours/LICENSE-MIT`

 * *Files identical despite different names*

### Comparing `opening_hours_py-0.6.7/local_dependencies/opening-hours/README.md` & `opening_hours_py-0.6.9/local_dependencies/opening-hours/README.md`

 * *Files identical despite different names*

### Comparing `opening_hours_py-0.6.7/local_dependencies/opening-hours/benches/benchmarks.rs` & `opening_hours_py-0.6.9/local_dependencies/opening-hours/benches/benchmarks.rs`

 * *Files identical despite different names*

### Comparing `opening_hours_py-0.6.7/local_dependencies/opening-hours/build.rs` & `opening_hours_py-0.6.9/local_dependencies/opening-hours/build.rs`

 * *Files identical despite different names*

### Comparing `opening_hours_py-0.6.7/local_dependencies/opening-hours/data/holidays.txt` & `opening_hours_py-0.6.9/local_dependencies/opening-hours/data/holidays.txt`

 * *Files identical despite different names*

### Comparing `opening_hours_py-0.6.7/local_dependencies/opening-hours/scripts/check-version.py` & `opening_hours_py-0.6.9/local_dependencies/opening-hours/scripts/check-version.py`

 * *Files identical despite different names*

### Comparing `opening_hours_py-0.6.7/local_dependencies/opening-hours/scripts/generate-holidays.py` & `opening_hours_py-0.6.9/local_dependencies/opening-hours/scripts/generate-holidays.py`

 * *Files identical despite different names*

### Comparing `opening_hours_py-0.6.7/local_dependencies/opening-hours/scripts/poetry.lock` & `opening_hours_py-0.6.9/local_dependencies/opening-hours/scripts/poetry.lock`

 * *Files identical despite different names*

### Comparing `opening_hours_py-0.6.7/local_dependencies/opening-hours/src/bin/schedule.rs` & `opening_hours_py-0.6.9/local_dependencies/opening-hours/src/bin/schedule.rs`

 * *Files identical despite different names*

### Comparing `opening_hours_py-0.6.7/local_dependencies/opening-hours/src/date_filter.rs` & `opening_hours_py-0.6.9/local_dependencies/opening-hours/src/date_filter.rs`

 * *Files identical despite different names*

### Comparing `opening_hours_py-0.6.7/local_dependencies/opening-hours/src/opening_hours.rs` & `opening_hours_py-0.6.9/local_dependencies/opening-hours/src/opening_hours.rs`

 * *Files identical despite different names*

### Comparing `opening_hours_py-0.6.7/local_dependencies/opening-hours/src/schedule.rs` & `opening_hours_py-0.6.9/local_dependencies/opening-hours/src/schedule.rs`

 * *Files identical despite different names*

### Comparing `opening_hours_py-0.6.7/local_dependencies/opening-hours/src/tests/data/sample.txt` & `opening_hours_py-0.6.9/local_dependencies/opening-hours/src/tests/data/sample.txt`

 * *Files identical despite different names*

### Comparing `opening_hours_py-0.6.7/local_dependencies/opening-hours/src/tests/holiday_selector.rs` & `opening_hours_py-0.6.9/local_dependencies/opening-hours/src/tests/holiday_selector.rs`

 * *Files identical despite different names*

### Comparing `opening_hours_py-0.6.7/local_dependencies/opening-hours/src/tests/issues.rs` & `opening_hours_py-0.6.9/local_dependencies/opening-hours/src/tests/issues.rs`

 * *Files identical despite different names*

### Comparing `opening_hours_py-0.6.7/local_dependencies/opening-hours/src/tests/mod.rs` & `opening_hours_py-0.6.9/local_dependencies/opening-hours/src/tests/mod.rs`

 * *Files identical despite different names*

### Comparing `opening_hours_py-0.6.7/local_dependencies/opening-hours/src/tests/month_selector.rs` & `opening_hours_py-0.6.9/local_dependencies/opening-hours/src/tests/month_selector.rs`

 * *Files identical despite different names*

### Comparing `opening_hours_py-0.6.7/local_dependencies/opening-hours/src/tests/next_change.rs` & `opening_hours_py-0.6.9/local_dependencies/opening-hours/src/tests/next_change.rs`

 * *Files identical despite different names*

### Comparing `opening_hours_py-0.6.7/local_dependencies/opening-hours/src/tests/rules.rs` & `opening_hours_py-0.6.9/local_dependencies/opening-hours/src/tests/rules.rs`

 * *Files identical despite different names*

### Comparing `opening_hours_py-0.6.7/local_dependencies/opening-hours/src/tests/selective.rs` & `opening_hours_py-0.6.9/local_dependencies/opening-hours/src/tests/selective.rs`

 * *Files identical despite different names*

### Comparing `opening_hours_py-0.6.7/local_dependencies/opening-hours/src/tests/time_selector.rs` & `opening_hours_py-0.6.9/local_dependencies/opening-hours/src/tests/time_selector.rs`

 * *Files identical despite different names*

### Comparing `opening_hours_py-0.6.7/local_dependencies/opening-hours/src/tests/week_selector.rs` & `opening_hours_py-0.6.9/local_dependencies/opening-hours/src/tests/week_selector.rs`

 * *Files identical despite different names*

### Comparing `opening_hours_py-0.6.7/local_dependencies/opening-hours/src/tests/weekday_selector.rs` & `opening_hours_py-0.6.9/local_dependencies/opening-hours/src/tests/weekday_selector.rs`

 * *Files identical despite different names*

### Comparing `opening_hours_py-0.6.7/local_dependencies/opening-hours/src/tests/year_selector.rs` & `opening_hours_py-0.6.9/local_dependencies/opening-hours/src/tests/year_selector.rs`

 * *Files identical despite different names*

### Comparing `opening_hours_py-0.6.7/local_dependencies/opening-hours/src/time_filter.rs` & `opening_hours_py-0.6.9/local_dependencies/opening-hours/src/time_filter.rs`

 * *Files identical despite different names*

### Comparing `opening_hours_py-0.6.7/local_dependencies/opening-hours/src/utils/range.rs` & `opening_hours_py-0.6.9/local_dependencies/opening-hours/src/utils/range.rs`

 * *Files identical despite different names*

### Comparing `opening_hours_py-0.6.7/local_dependencies/opening-hours-syntax/Cargo.toml` & `opening_hours_py-0.6.9/local_dependencies/opening-hours-syntax/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "opening-hours-syntax"
-version = "0.6.7"
+version = "0.6.9"
 authors = ["Rémi Dupré <remi@dupre.io>"]
 license = "MIT OR Apache-2.0"
 readme = "README.md"
 repository = "https://github.com/remi-dupre/opening-hours-rs"
 documentation = "https://docs.rs/opening-hours-syntax"
 homepage = "https://github.com/remi-dupre/opening-hours-rs/tree/master/opening-hours-syntax"
 description = "A parser for opening_hours fields in OpenStreetMap."
```

### Comparing `opening_hours_py-0.6.7/local_dependencies/opening-hours-syntax/LICENSE-APACHE` & `opening_hours_py-0.6.9/local_dependencies/opening-hours-syntax/LICENSE-APACHE`

 * *Files identical despite different names*

### Comparing `opening_hours_py-0.6.7/local_dependencies/opening-hours-syntax/LICENSE-MIT` & `opening_hours_py-0.6.9/local_dependencies/opening-hours-syntax/LICENSE-MIT`

 * *Files identical despite different names*

### Comparing `opening_hours_py-0.6.7/local_dependencies/opening-hours-syntax/README.md` & `opening_hours_py-0.6.9/local_dependencies/opening-hours-syntax/README.md`

 * *Files identical despite different names*

### Comparing `opening_hours_py-0.6.7/local_dependencies/opening-hours-syntax/src/error.rs` & `opening_hours_py-0.6.9/local_dependencies/opening-hours-syntax/src/error.rs`

 * *Files identical despite different names*

### Comparing `opening_hours_py-0.6.7/local_dependencies/opening-hours-syntax/src/extended_time.rs` & `opening_hours_py-0.6.9/local_dependencies/opening-hours-syntax/src/extended_time.rs`

 * *Files identical despite different names*

### Comparing `opening_hours_py-0.6.7/local_dependencies/opening-hours-syntax/src/grammar.pest` & `opening_hours_py-0.6.9/local_dependencies/opening-hours-syntax/src/grammar.pest`

 * *Files identical despite different names*

### Comparing `opening_hours_py-0.6.7/local_dependencies/opening-hours-syntax/src/lib.rs` & `opening_hours_py-0.6.9/local_dependencies/opening-hours-syntax/src/lib.rs`

 * *Files identical despite different names*

### Comparing `opening_hours_py-0.6.7/local_dependencies/opening-hours-syntax/src/parser.rs` & `opening_hours_py-0.6.9/local_dependencies/opening-hours-syntax/src/parser.rs`

 * *Files identical despite different names*

### Comparing `opening_hours_py-0.6.7/local_dependencies/opening-hours-syntax/src/rules/day.rs` & `opening_hours_py-0.6.9/local_dependencies/opening-hours-syntax/src/rules/day.rs`

 * *Files identical despite different names*

### Comparing `opening_hours_py-0.6.7/local_dependencies/opening-hours-syntax/src/rules/mod.rs` & `opening_hours_py-0.6.9/local_dependencies/opening-hours-syntax/src/rules/mod.rs`

 * *Files identical despite different names*

### Comparing `opening_hours_py-0.6.7/local_dependencies/opening-hours-syntax/src/rules/time.rs` & `opening_hours_py-0.6.9/local_dependencies/opening-hours-syntax/src/rules/time.rs`

 * *Files identical despite different names*

### Comparing `opening_hours_py-0.6.7/local_dependencies/opening-hours-syntax/src/sorted_vec.rs` & `opening_hours_py-0.6.9/local_dependencies/opening-hours-syntax/src/sorted_vec.rs`

 * *Files identical despite different names*

### Comparing `opening_hours_py-0.6.7/Cargo.toml` & `opening_hours_py-0.6.9/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "opening-hours-py"
-version = "0.6.7"
+version = "0.6.9"
 authors = ["Rémi Dupré <remi@dupre.io>"]
 license = "MIT OR Apache-2.0"
 readme = "README.md"
 repository = "https://github.com/remi-dupre/opening-hours-rs"
 documentation = "https://remi-dupre.github.io/opening-hours-rs/opening_hours.html"
 homepage = "https://github.com/remi-dupre/opening-hours-rs/tree/master/python"
 description = "A parser and toolkit for the opening_hours in OpenStreetMap written in Rust."
```

### Comparing `opening_hours_py-0.6.7/LICENSE-APACHE` & `opening_hours_py-0.6.9/LICENSE-APACHE`

 * *Files identical despite different names*

### Comparing `opening_hours_py-0.6.7/LICENSE-MIT` & `opening_hours_py-0.6.9/LICENSE-MIT`

 * *Files identical despite different names*

### Comparing `opening_hours_py-0.6.7/README.md` & `opening_hours_py-0.6.9/README.md`

 * *Files identical despite different names*

### Comparing `opening_hours_py-0.6.7/poetry.lock` & `opening_hours_py-0.6.9/poetry.lock`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,10 @@
 # This file is automatically @generated by Poetry 1.5.1 and should not be changed by hand.
 
 [[package]]
-name = "astunparse"
-version = "1.6.3"
-description = "An AST unparser for Python"
-optional = false
-python-versions = "*"
-files = [
-    {file = "astunparse-1.6.3-py2.py3-none-any.whl", hash = "sha256:c2652417f2c8b5bb325c885ae329bdf3f86424075c4fd1a128674bc6fba4b8e8"},
-    {file = "astunparse-1.6.3.tar.gz", hash = "sha256:5ad93a8456f0d084c3456d059fd9a92cce667963232cbf763eac3bc5b7940872"},
-]
-
-[package.dependencies]
-six = ">=1.6.1,<2.0"
-wheel = ">=0.23.0,<1.0"
-
-[[package]]
 name = "jinja2"
 version = "3.1.2"
 description = "A very fast and expressive template engine."
 optional = false
 python-versions = ">=3.7"
 files = [
     {file = "Jinja2-3.1.2-py3-none-any.whl", hash = "sha256:6088930bfe239f0e6710546ab9c19c9ef35e29792895fed6e6e31a023a182a61"},
@@ -128,15 +113,14 @@
 python-versions = ">=3.7"
 files = [
     {file = "pdoc-12.3.1-py3-none-any.whl", hash = "sha256:c3f24f31286e634de9c76fa6e67bd5c0c5e74360b41dc91e6b82499831eb52d8"},
     {file = "pdoc-12.3.1.tar.gz", hash = "sha256:453236f225feddb8a9071428f1982a78d74b9b3da4bc4433aedb64dbd0cc87ab"},
 ]
 
 [package.dependencies]
-astunparse = {version = "*", markers = "python_version < \"3.9\""}
 Jinja2 = ">=2.11.0"
 MarkupSafe = "*"
 pygments = ">=2.12.0"
 
 [package.extras]
 dev = ["black", "hypothesis", "mypy", "pytest", "pytest-cov", "pytest-timeout", "ruff", "tox", "types-pygments"]
 
@@ -151,46 +135,21 @@
     {file = "Pygments-2.15.1.tar.gz", hash = "sha256:8ace4d3c1dd481894b2005f560ead0f9f19ee64fe983366be1a21e171d12775c"},
 ]
 
 [package.extras]
 plugins = ["importlib-metadata"]
 
 [[package]]
-name = "six"
-version = "1.16.0"
-description = "Python 2 and 3 compatibility utilities"
-optional = false
-python-versions = ">=2.7, !=3.0.*, !=3.1.*, !=3.2.*"
-files = [
-    {file = "six-1.16.0-py2.py3-none-any.whl", hash = "sha256:8abb2f1d86890a2dfb989f9a77cfcfd3e47c2a354b01111771326f8aa26e0254"},
-    {file = "six-1.16.0.tar.gz", hash = "sha256:1e61c37477a1626458e36f7b1d82aa5c9b094fa4802892072e49de9c60c4c926"},
-]
-
-[[package]]
 name = "tomli"
 version = "2.0.1"
 description = "A lil' TOML parser"
 optional = false
 python-versions = ">=3.7"
 files = [
     {file = "tomli-2.0.1-py3-none-any.whl", hash = "sha256:939de3e7a6161af0c887ef91b7d41a53e7c5a1ca976325f429cb46ea9bc30ecc"},
     {file = "tomli-2.0.1.tar.gz", hash = "sha256:de526c12914f0c550d15924c62d72abc48d6fe7364aa87328337a31007fe8a4f"},
 ]
 
-[[package]]
-name = "wheel"
-version = "0.40.0"
-description = "A built-package format for Python"
-optional = false
-python-versions = ">=3.7"
-files = [
-    {file = "wheel-0.40.0-py3-none-any.whl", hash = "sha256:d236b20e7cb522daf2390fa84c55eea81c5c30190f90f29ae2ca1ad8355bf247"},
-    {file = "wheel-0.40.0.tar.gz", hash = "sha256:cd1196f3faee2b31968d626e1731c94f99cbdb67cf5a46e4f5656cbee7738873"},
-]
-
-[package.extras]
-test = ["pytest (>=6.0.0)"]
-
 [metadata]
 lock-version = "2.0"
-python-versions = "^3.8"
-content-hash = "217c1268eb52923df9488713fdd4cedd827a865ac7151202cbaa6bf3de881d62"
+python-versions = "^3.9"
+content-hash = "332291e13df8556b5ef6194f642affff2f47b0b4e160db01447c3a9e3039ae00"
```

### Comparing `opening_hours_py-0.6.7/src/errors.rs` & `opening_hours_py-0.6.9/src/errors.rs`

 * *Files identical despite different names*

### Comparing `opening_hours_py-0.6.7/src/lib.rs` & `opening_hours_py-0.6.9/src/lib.rs`

 * *Files identical despite different names*

### Comparing `opening_hours_py-0.6.7/src/types.rs` & `opening_hours_py-0.6.9/src/types.rs`

 * *Files identical despite different names*

### Comparing `opening_hours_py-0.6.7/Cargo.lock` & `opening_hours_py-0.6.9/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -33,17 +33,17 @@
 name = "anstyle"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "41ed9a86bf92ae6580e0a31281f65a1b1d867c0cc68d5346e2ae128dddfa6a7d"
 
 [[package]]
 name = "arbitrary"
-version = "0.4.7"
+version = "1.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "db55d72333851e17d572bec876e390cd3b11eb1ef53ae821dd9f3b653d2b4569"
+checksum = "e2d098ff73c1ca148721f37baad5ea6a465a13f9573aba8641fbbbae8164a54e"
 dependencies = [
  "derive_arbitrary",
 ]
 
 [[package]]
 name = "autocfg"
 version = "1.1.0"
@@ -78,14 +78,17 @@
 checksum = "37b2a672a2cb129a2e41c10b1224bb368f9f37a2b16b612598138befd7b37eb5"
 
 [[package]]
 name = "cc"
 version = "1.0.79"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "50d30906286121d95be3d479533b458f87493b30a4b5f79a607db8f5d11aa91f"
+dependencies = [
+ "jobserver",
+]
 
 [[package]]
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
@@ -155,15 +158,15 @@
 name = "clap_lex"
 version = "0.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2da6da31387c7e4ef160ffab6d5e7f00c42626fe39aea70a7b0f1773f7dd6c1b"
 
 [[package]]
 name = "compact-calendar"
-version = "0.6.7"
+version = "0.6.9"
 dependencies = [
  "chrono",
 ]
 
 [[package]]
 name = "core-foundation-sys"
 version = "0.8.4"
@@ -275,21 +278,21 @@
 dependencies = [
  "generic-array",
  "typenum",
 ]
 
 [[package]]
 name = "derive_arbitrary"
-version = "0.4.7"
+version = "1.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b1a012b5e473dc912f0db0546a1c9c6a194ce8494feb66fa0237160926f9e0e6"
+checksum = "53e0efad4403bfc52dc201159c4b842a246a14b98c64b55dfd0f2d89729dfeb8"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 1.0.109",
+ "syn 2.0.18",
 ]
 
 [[package]]
 name = "digest"
 version = "0.10.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9ed9a281f7bc9b7576e61468ba615a66a5c8cfdff42420a70aa82701a3b1e292"
@@ -440,14 +443,23 @@
 [[package]]
 name = "itoa"
 version = "1.0.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "453ad9f582a441959e5f0d088b02ce04cfe8d51a8eaf077f12ac6d3e94164ca6"
 
 [[package]]
+name = "jobserver"
+version = "0.1.26"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "936cfd212a0155903bcbc060e316fb6cc7cbf2e1907329391ebadc1fe0ce77c2"
+dependencies = [
+ "libc",
+]
+
+[[package]]
 name = "js-sys"
 version = "0.3.64"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c5f195fe497f702db0f318b07fdd68edb16955aed830df8363d837542f8f935a"
 dependencies = [
  "wasm-bindgen",
 ]
@@ -456,20 +468,21 @@
 name = "libc"
 version = "0.2.146"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f92be4933c13fd498862a9e02a3055f8a8d9c039ce33db97306fd5a6caa7f29b"
 
 [[package]]
 name = "libfuzzer-sys"
-version = "0.3.5"
+version = "0.4.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fcf184a4b6b274f82a5df6b357da6055d3e82272327bba281c28bbba6f1664ef"
+checksum = "beb09950ae85a0a94b27676cccf37da5ff13f27076aa1adbc6545dd0d0e1bd4e"
 dependencies = [
  "arbitrary",
  "cc",
+ "once_cell",
 ]
 
 [[package]]
 name = "linux-raw-sys"
 version = "0.3.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ef53942eb7bf7ff43a617b3e2c1c4a5ecf5944a7c1bc12d7ee39bbb15e5c1519"
@@ -537,37 +550,37 @@
 name = "oorandom"
 version = "11.1.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0ab1bc2a289d34bd04a330323ac98a1b4bc82c9d9fcb1e66b63caa84da26b575"
 
 [[package]]
 name = "opening-hours"
-version = "0.6.7"
+version = "0.6.9"
 dependencies = [
  "chrono",
  "compact-calendar",
  "criterion",
  "flate2",
  "once_cell",
  "opening-hours-syntax",
 ]
 
 [[package]]
 name = "opening-hours-py"
-version = "0.6.7"
+version = "0.6.9"
 dependencies = [
  "chrono",
  "opening-hours",
  "opening-hours-syntax",
  "pyo3",
 ]
 
 [[package]]
 name = "opening-hours-syntax"
-version = "0.6.7"
+version = "0.6.9"
 dependencies = [
  "chrono",
  "pest",
  "pest_derive",
 ]
 
 [[package]]
```

### Comparing `opening_hours_py-0.6.7/PKG-INFO` & `opening_hours_py-0.6.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opening-hours-py
-Version: 0.6.7
+Version: 0.6.9
 Summary: A parser and toolkit for the opening_hours in OpenStreetMap written in Rust.
 Home-Page: https://github.com/remi-dupre/opening-hours-rs/tree/master/python
 Author: Rémi Dupré <remi@dupre.io>
 Author-email: Rémi Dupré <remi@dupre.io>
 License: MIT OR Apache-2.0
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 Project-URL: Source Code, https://github.com/remi-dupre/opening-hours-rs
```

