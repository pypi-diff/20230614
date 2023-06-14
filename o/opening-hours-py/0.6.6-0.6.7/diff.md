# Comparing `tmp/opening_hours_py-0.6.6.tar.gz` & `tmp/opening_hours_py-0.6.7.tar.gz`

## Comparing `opening_hours_py-0.6.6.tar` & `opening_hours_py-0.6.7.tar`

### file list

```diff
@@ -1,68 +1,68 @@
--rw-r--r--   0        0        0      514 1970-01-01 00:00:00.000000 opening_hours_py-0.6.6/local_dependencies/compact-calendar/Cargo.toml
--rw-r--r--   0     1001      123     1588 2023-06-14 12:18:47.000000 opening_hours_py-0.6.6/local_dependencies/compact-calendar/README.md
--rw-r--r--   0     1001      123    23597 2023-06-14 12:18:47.000000 opening_hours_py-0.6.6/local_dependencies/compact-calendar/src/lib.rs
--rw-r--r--   0        0        0      935 1970-01-01 00:00:00.000000 opening_hours_py-0.6.6/local_dependencies/opening-hours/Cargo.toml
--rw-r--r--   0     1001      123       86 2023-06-14 12:18:47.000000 opening_hours_py-0.6.6/local_dependencies/opening-hours/.github/codecov.yml
--rw-r--r--   0     1001      123     2693 2023-06-14 12:18:47.000000 opening_hours_py-0.6.6/local_dependencies/opening-hours/.github/workflows/deploy.yml
--rw-r--r--   0     1001      123     2326 2023-06-14 12:18:47.000000 opening_hours_py-0.6.6/local_dependencies/opening-hours/.github/workflows/tests.yml
--rw-r--r--   0     1001      123       49 2023-06-14 12:18:47.000000 opening_hours_py-0.6.6/local_dependencies/opening-hours/.gitignore
--rw-r--r--   0     1001      123       22 2023-06-14 12:18:47.000000 opening_hours_py-0.6.6/local_dependencies/opening-hours/.rustfmt.toml
--rw-r--r--   0     1001      123    29444 2023-06-14 12:18:47.000000 opening_hours_py-0.6.6/local_dependencies/opening-hours/Cargo.lock
--rw-r--r--   0     1001      123    10847 2023-06-14 12:18:47.000000 opening_hours_py-0.6.6/local_dependencies/opening-hours/LICENSE-APACHE
--rw-r--r--   0     1001      123     1056 2023-06-14 12:18:47.000000 opening_hours_py-0.6.6/local_dependencies/opening-hours/LICENSE-MIT
--rw-r--r--   0     1001      123     2800 2023-06-14 12:18:47.000000 opening_hours_py-0.6.6/local_dependencies/opening-hours/README.md
--rw-r--r--   0     1001      123     1996 2023-06-14 12:18:47.000000 opening_hours_py-0.6.6/local_dependencies/opening-hours/benches/benchmarks.rs
--rw-r--r--   0     1001      123     2368 2023-06-14 12:18:47.000000 opening_hours_py-0.6.6/local_dependencies/opening-hours/build.rs
--rw-r--r--   0     1001      123  4657878 2023-06-14 12:18:47.000000 opening_hours_py-0.6.6/local_dependencies/opening-hours/data/holidays.txt
--rwxr-xr-x   0     1001      123     3275 2023-06-14 12:18:47.000000 opening_hours_py-0.6.6/local_dependencies/opening-hours/scripts/check-version.py
--rwxr-xr-x   0     1001      123     1092 2023-06-14 12:18:47.000000 opening_hours_py-0.6.6/local_dependencies/opening-hours/scripts/generate-holidays.py
--rw-r--r--   0     1001      123    12546 2023-06-14 12:18:47.000000 opening_hours_py-0.6.6/local_dependencies/opening-hours/scripts/poetry.lock
--rw-r--r--   0     1001      123      428 2023-06-14 12:18:47.000000 opening_hours_py-0.6.6/local_dependencies/opening-hours/scripts/pyproject.toml
--rw-r--r--   0     1001      123     1370 2023-06-14 12:18:47.000000 opening_hours_py-0.6.6/local_dependencies/opening-hours/src/bin/schedule.rs
--rw-r--r--   0     1001      123    12893 2023-06-14 12:18:47.000000 opening_hours_py-0.6.6/local_dependencies/opening-hours/src/date_filter.rs
--rw-r--r--   0     1001      123      400 2023-06-14 12:18:47.000000 opening_hours_py-0.6.6/local_dependencies/opening-hours/src/lib.rs
--rw-r--r--   0     1001      123    11396 2023-06-14 12:18:47.000000 opening_hours_py-0.6.6/local_dependencies/opening-hours/src/opening_hours.rs
--rw-r--r--   0     1001      123     6628 2023-06-14 12:18:47.000000 opening_hours_py-0.6.6/local_dependencies/opening-hours/src/schedule.rs
--rw-r--r--   0     1001      123     9791 2023-06-14 12:18:47.000000 opening_hours_py-0.6.6/local_dependencies/opening-hours/src/tests/data/sample.txt
--rw-r--r--   0     1001      123      824 2023-06-14 12:18:47.000000 opening_hours_py-0.6.6/local_dependencies/opening-hours/src/tests/holiday_selector.rs
--rw-r--r--   0     1001      123      905 2023-06-14 12:18:47.000000 opening_hours_py-0.6.6/local_dependencies/opening-hours/src/tests/issues.rs
--rw-r--r--   0     1001      123     2501 2023-06-14 12:18:47.000000 opening_hours_py-0.6.6/local_dependencies/opening-hours/src/tests/mod.rs
--rw-r--r--   0     1001      123     1487 2023-06-14 12:18:47.000000 opening_hours_py-0.6.6/local_dependencies/opening-hours/src/tests/month_selector.rs
--rw-r--r--   0     1001      123     1528 2023-06-14 12:18:47.000000 opening_hours_py-0.6.6/local_dependencies/opening-hours/src/tests/next_change.rs
--rw-r--r--   0     1001      123      497 2023-06-14 12:18:47.000000 opening_hours_py-0.6.6/local_dependencies/opening-hours/src/tests/next_change_hint.rs
--rw-r--r--   0     1001      123      339 2023-06-14 12:18:47.000000 opening_hours_py-0.6.6/local_dependencies/opening-hours/src/tests/parser.rs
--rw-r--r--   0     1001      123     2790 2023-06-14 12:18:47.000000 opening_hours_py-0.6.6/local_dependencies/opening-hours/src/tests/rules.rs
--rw-r--r--   0     1001      123     3243 2023-06-14 12:18:47.000000 opening_hours_py-0.6.6/local_dependencies/opening-hours/src/tests/selective.rs
--rw-r--r--   0     1001      123     1598 2023-06-14 12:18:47.000000 opening_hours_py-0.6.6/local_dependencies/opening-hours/src/tests/time_selector.rs
--rw-r--r--   0     1001      123     1176 2023-06-14 12:18:47.000000 opening_hours_py-0.6.6/local_dependencies/opening-hours/src/tests/week_selector.rs
--rw-r--r--   0     1001      123     2541 2023-06-14 12:18:47.000000 opening_hours_py-0.6.6/local_dependencies/opening-hours/src/tests/weekday_selector.rs
--rw-r--r--   0     1001      123     1419 2023-06-14 12:18:47.000000 opening_hours_py-0.6.6/local_dependencies/opening-hours/src/tests/year_selector.rs
--rw-r--r--   0     1001      123     3287 2023-06-14 12:18:47.000000 opening_hours_py-0.6.6/local_dependencies/opening-hours/src/time_filter.rs
--rw-r--r--   0     1001      123       22 2023-06-14 12:18:47.000000 opening_hours_py-0.6.6/local_dependencies/opening-hours/src/utils/mod.rs
--rw-r--r--   0     1001      123     3872 2023-06-14 12:18:47.000000 opening_hours_py-0.6.6/local_dependencies/opening-hours/src/utils/range.rs
--rw-r--r--   0        0        0      551 1970-01-01 00:00:00.000000 opening_hours_py-0.6.6/local_dependencies/opening-hours-syntax/Cargo.toml
--rw-r--r--   0     1001      123    10847 2023-06-14 12:18:47.000000 opening_hours_py-0.6.6/local_dependencies/opening-hours-syntax/LICENSE-APACHE
--rw-r--r--   0     1001      123     1056 2023-06-14 12:18:47.000000 opening_hours_py-0.6.6/local_dependencies/opening-hours-syntax/LICENSE-MIT
--rw-r--r--   0     1001      123      874 2023-06-14 12:18:47.000000 opening_hours_py-0.6.6/local_dependencies/opening-hours-syntax/README.md
--rw-r--r--   0     1001      123      859 2023-06-14 12:18:47.000000 opening_hours_py-0.6.6/local_dependencies/opening-hours-syntax/src/error.rs
--rw-r--r--   0     1001      123     2087 2023-06-14 12:18:47.000000 opening_hours_py-0.6.6/local_dependencies/opening-hours-syntax/src/extended_time.rs
--rw-r--r--   0     1001      123     6513 2023-06-14 12:18:47.000000 opening_hours_py-0.6.6/local_dependencies/opening-hours-syntax/src/grammar.pest
--rw-r--r--   0     1001      123      810 2023-06-14 12:18:47.000000 opening_hours_py-0.6.6/local_dependencies/opening-hours-syntax/src/lib.rs
--rw-r--r--   0     1001      123    24312 2023-06-14 12:18:47.000000 opening_hours_py-0.6.6/local_dependencies/opening-hours-syntax/src/parser.rs
--rw-r--r--   0     1001      123     4206 2023-06-14 12:18:47.000000 opening_hours_py-0.6.6/local_dependencies/opening-hours-syntax/src/rules/day.rs
--rw-r--r--   0     1001      123      584 2023-06-14 12:18:47.000000 opening_hours_py-0.6.6/local_dependencies/opening-hours-syntax/src/rules/mod.rs
--rw-r--r--   0     1001      123     1381 2023-06-14 12:18:47.000000 opening_hours_py-0.6.6/local_dependencies/opening-hours-syntax/src/rules/time.rs
--rw-r--r--   0     1001      123     4048 2023-06-14 12:18:47.000000 opening_hours_py-0.6.6/local_dependencies/opening-hours-syntax/src/sorted_vec.rs
--rw-r--r--   0        0        0      824 1970-01-01 00:00:00.000000 opening_hours_py-0.6.6/Cargo.toml
--rw-r--r--   0     1001      123       40 2023-06-14 12:18:47.000000 opening_hours_py-0.6.6/.gitignore
--rw-r--r--   0     1001      123    10847 2023-06-14 12:18:47.000000 opening_hours_py-0.6.6/LICENSE-APACHE
--rw-r--r--   0     1001      123     1056 2023-06-14 12:18:47.000000 opening_hours_py-0.6.6/LICENSE-MIT
--rw-r--r--   0     1001      123     1718 2023-06-14 12:18:47.000000 opening_hours_py-0.6.6/README.md
--rw-r--r--   0     1001      123    12755 2023-06-14 12:18:47.000000 opening_hours_py-0.6.6/poetry.lock
--rw-r--r--   0     1001      123      374 2023-06-14 12:18:47.000000 opening_hours_py-0.6.6/pyproject.toml
--rwxr-xr-x   0     1001      123      490 2023-06-14 12:18:47.000000 opening_hours_py-0.6.6/run_doctests.py
--rw-r--r--   0     1001      123      692 2023-06-14 12:18:47.000000 opening_hours_py-0.6.6/src/errors.rs
--rw-r--r--   0     1001      123     6474 2023-06-14 12:18:47.000000 opening_hours_py-0.6.6/src/lib.rs
--rw-r--r--   0     1001      123     4967 2023-06-14 12:18:47.000000 opening_hours_py-0.6.6/src/types.rs
--rw-r--r--   0     1001      123    29444 2023-06-14 12:18:47.000000 opening_hours_py-0.6.6/Cargo.lock
--rw-r--r--   0        0        0     2191 1970-01-01 00:00:00.000000 opening_hours_py-0.6.6/PKG-INFO
+-rw-r--r--   0        0        0      514 1970-01-01 00:00:00.000000 opening_hours_py-0.6.7/local_dependencies/compact-calendar/Cargo.toml
+-rw-r--r--   0     1001      123     1588 2023-06-14 14:01:22.000000 opening_hours_py-0.6.7/local_dependencies/compact-calendar/README.md
+-rw-r--r--   0     1001      123    23597 2023-06-14 14:01:22.000000 opening_hours_py-0.6.7/local_dependencies/compact-calendar/src/lib.rs
+-rw-r--r--   0        0        0      935 1970-01-01 00:00:00.000000 opening_hours_py-0.6.7/local_dependencies/opening-hours/Cargo.toml
+-rw-r--r--   0     1001      123       86 2023-06-14 14:01:22.000000 opening_hours_py-0.6.7/local_dependencies/opening-hours/.github/codecov.yml
+-rw-r--r--   0     1001      123     2837 2023-06-14 14:01:22.000000 opening_hours_py-0.6.7/local_dependencies/opening-hours/.github/workflows/deploy.yml
+-rw-r--r--   0     1001      123     2325 2023-06-14 14:01:22.000000 opening_hours_py-0.6.7/local_dependencies/opening-hours/.github/workflows/tests.yml
+-rw-r--r--   0     1001      123       49 2023-06-14 14:01:22.000000 opening_hours_py-0.6.7/local_dependencies/opening-hours/.gitignore
+-rw-r--r--   0     1001      123       22 2023-06-14 14:01:22.000000 opening_hours_py-0.6.7/local_dependencies/opening-hours/.rustfmt.toml
+-rw-r--r--   0     1001      123    29444 2023-06-14 14:01:22.000000 opening_hours_py-0.6.7/local_dependencies/opening-hours/Cargo.lock
+-rw-r--r--   0     1001      123    10847 2023-06-14 14:01:22.000000 opening_hours_py-0.6.7/local_dependencies/opening-hours/LICENSE-APACHE
+-rw-r--r--   0     1001      123     1056 2023-06-14 14:01:22.000000 opening_hours_py-0.6.7/local_dependencies/opening-hours/LICENSE-MIT
+-rw-r--r--   0     1001      123     2800 2023-06-14 14:01:22.000000 opening_hours_py-0.6.7/local_dependencies/opening-hours/README.md
+-rw-r--r--   0     1001      123     1996 2023-06-14 14:01:22.000000 opening_hours_py-0.6.7/local_dependencies/opening-hours/benches/benchmarks.rs
+-rw-r--r--   0     1001      123     2368 2023-06-14 14:01:22.000000 opening_hours_py-0.6.7/local_dependencies/opening-hours/build.rs
+-rw-r--r--   0     1001      123  4657878 2023-06-14 14:01:22.000000 opening_hours_py-0.6.7/local_dependencies/opening-hours/data/holidays.txt
+-rwxr-xr-x   0     1001      123     3275 2023-06-14 14:01:22.000000 opening_hours_py-0.6.7/local_dependencies/opening-hours/scripts/check-version.py
+-rwxr-xr-x   0     1001      123     1092 2023-06-14 14:01:22.000000 opening_hours_py-0.6.7/local_dependencies/opening-hours/scripts/generate-holidays.py
+-rw-r--r--   0     1001      123    12546 2023-06-14 14:01:22.000000 opening_hours_py-0.6.7/local_dependencies/opening-hours/scripts/poetry.lock
+-rw-r--r--   0     1001      123      428 2023-06-14 14:01:22.000000 opening_hours_py-0.6.7/local_dependencies/opening-hours/scripts/pyproject.toml
+-rw-r--r--   0     1001      123     1370 2023-06-14 14:01:22.000000 opening_hours_py-0.6.7/local_dependencies/opening-hours/src/bin/schedule.rs
+-rw-r--r--   0     1001      123    12893 2023-06-14 14:01:22.000000 opening_hours_py-0.6.7/local_dependencies/opening-hours/src/date_filter.rs
+-rw-r--r--   0     1001      123      400 2023-06-14 14:01:22.000000 opening_hours_py-0.6.7/local_dependencies/opening-hours/src/lib.rs
+-rw-r--r--   0     1001      123    11396 2023-06-14 14:01:22.000000 opening_hours_py-0.6.7/local_dependencies/opening-hours/src/opening_hours.rs
+-rw-r--r--   0     1001      123     6628 2023-06-14 14:01:22.000000 opening_hours_py-0.6.7/local_dependencies/opening-hours/src/schedule.rs
+-rw-r--r--   0     1001      123     9791 2023-06-14 14:01:22.000000 opening_hours_py-0.6.7/local_dependencies/opening-hours/src/tests/data/sample.txt
+-rw-r--r--   0     1001      123      824 2023-06-14 14:01:22.000000 opening_hours_py-0.6.7/local_dependencies/opening-hours/src/tests/holiday_selector.rs
+-rw-r--r--   0     1001      123      905 2023-06-14 14:01:22.000000 opening_hours_py-0.6.7/local_dependencies/opening-hours/src/tests/issues.rs
+-rw-r--r--   0     1001      123     2501 2023-06-14 14:01:22.000000 opening_hours_py-0.6.7/local_dependencies/opening-hours/src/tests/mod.rs
+-rw-r--r--   0     1001      123     1487 2023-06-14 14:01:22.000000 opening_hours_py-0.6.7/local_dependencies/opening-hours/src/tests/month_selector.rs
+-rw-r--r--   0     1001      123     1528 2023-06-14 14:01:22.000000 opening_hours_py-0.6.7/local_dependencies/opening-hours/src/tests/next_change.rs
+-rw-r--r--   0     1001      123      497 2023-06-14 14:01:22.000000 opening_hours_py-0.6.7/local_dependencies/opening-hours/src/tests/next_change_hint.rs
+-rw-r--r--   0     1001      123      339 2023-06-14 14:01:22.000000 opening_hours_py-0.6.7/local_dependencies/opening-hours/src/tests/parser.rs
+-rw-r--r--   0     1001      123     2790 2023-06-14 14:01:22.000000 opening_hours_py-0.6.7/local_dependencies/opening-hours/src/tests/rules.rs
+-rw-r--r--   0     1001      123     3243 2023-06-14 14:01:22.000000 opening_hours_py-0.6.7/local_dependencies/opening-hours/src/tests/selective.rs
+-rw-r--r--   0     1001      123     1598 2023-06-14 14:01:22.000000 opening_hours_py-0.6.7/local_dependencies/opening-hours/src/tests/time_selector.rs
+-rw-r--r--   0     1001      123     1176 2023-06-14 14:01:22.000000 opening_hours_py-0.6.7/local_dependencies/opening-hours/src/tests/week_selector.rs
+-rw-r--r--   0     1001      123     2541 2023-06-14 14:01:22.000000 opening_hours_py-0.6.7/local_dependencies/opening-hours/src/tests/weekday_selector.rs
+-rw-r--r--   0     1001      123     1419 2023-06-14 14:01:22.000000 opening_hours_py-0.6.7/local_dependencies/opening-hours/src/tests/year_selector.rs
+-rw-r--r--   0     1001      123     3287 2023-06-14 14:01:22.000000 opening_hours_py-0.6.7/local_dependencies/opening-hours/src/time_filter.rs
+-rw-r--r--   0     1001      123       22 2023-06-14 14:01:22.000000 opening_hours_py-0.6.7/local_dependencies/opening-hours/src/utils/mod.rs
+-rw-r--r--   0     1001      123     3872 2023-06-14 14:01:22.000000 opening_hours_py-0.6.7/local_dependencies/opening-hours/src/utils/range.rs
+-rw-r--r--   0        0        0      551 1970-01-01 00:00:00.000000 opening_hours_py-0.6.7/local_dependencies/opening-hours-syntax/Cargo.toml
+-rw-r--r--   0     1001      123    10847 2023-06-14 14:01:22.000000 opening_hours_py-0.6.7/local_dependencies/opening-hours-syntax/LICENSE-APACHE
+-rw-r--r--   0     1001      123     1056 2023-06-14 14:01:22.000000 opening_hours_py-0.6.7/local_dependencies/opening-hours-syntax/LICENSE-MIT
+-rw-r--r--   0     1001      123      874 2023-06-14 14:01:22.000000 opening_hours_py-0.6.7/local_dependencies/opening-hours-syntax/README.md
+-rw-r--r--   0     1001      123      859 2023-06-14 14:01:22.000000 opening_hours_py-0.6.7/local_dependencies/opening-hours-syntax/src/error.rs
+-rw-r--r--   0     1001      123     2087 2023-06-14 14:01:22.000000 opening_hours_py-0.6.7/local_dependencies/opening-hours-syntax/src/extended_time.rs
+-rw-r--r--   0     1001      123     6513 2023-06-14 14:01:22.000000 opening_hours_py-0.6.7/local_dependencies/opening-hours-syntax/src/grammar.pest
+-rw-r--r--   0     1001      123      810 2023-06-14 14:01:22.000000 opening_hours_py-0.6.7/local_dependencies/opening-hours-syntax/src/lib.rs
+-rw-r--r--   0     1001      123    24312 2023-06-14 14:01:22.000000 opening_hours_py-0.6.7/local_dependencies/opening-hours-syntax/src/parser.rs
+-rw-r--r--   0     1001      123     4206 2023-06-14 14:01:22.000000 opening_hours_py-0.6.7/local_dependencies/opening-hours-syntax/src/rules/day.rs
+-rw-r--r--   0     1001      123      584 2023-06-14 14:01:22.000000 opening_hours_py-0.6.7/local_dependencies/opening-hours-syntax/src/rules/mod.rs
+-rw-r--r--   0     1001      123     1381 2023-06-14 14:01:22.000000 opening_hours_py-0.6.7/local_dependencies/opening-hours-syntax/src/rules/time.rs
+-rw-r--r--   0     1001      123     4048 2023-06-14 14:01:22.000000 opening_hours_py-0.6.7/local_dependencies/opening-hours-syntax/src/sorted_vec.rs
+-rw-r--r--   0        0        0      824 1970-01-01 00:00:00.000000 opening_hours_py-0.6.7/Cargo.toml
+-rw-r--r--   0     1001      123       40 2023-06-14 14:01:22.000000 opening_hours_py-0.6.7/.gitignore
+-rw-r--r--   0     1001      123    10847 2023-06-14 14:01:22.000000 opening_hours_py-0.6.7/LICENSE-APACHE
+-rw-r--r--   0     1001      123     1056 2023-06-14 14:01:22.000000 opening_hours_py-0.6.7/LICENSE-MIT
+-rw-r--r--   0     1001      123     1871 2023-06-14 14:01:22.000000 opening_hours_py-0.6.7/README.md
+-rw-r--r--   0     1001      123    14166 2023-06-14 14:01:22.000000 opening_hours_py-0.6.7/poetry.lock
+-rw-r--r--   0     1001      123      374 2023-06-14 14:01:22.000000 opening_hours_py-0.6.7/pyproject.toml
+-rwxr-xr-x   0     1001      123      490 2023-06-14 14:01:22.000000 opening_hours_py-0.6.7/run_doctests.py
+-rw-r--r--   0     1001      123      692 2023-06-14 14:01:22.000000 opening_hours_py-0.6.7/src/errors.rs
+-rw-r--r--   0     1001      123     6474 2023-06-14 14:01:22.000000 opening_hours_py-0.6.7/src/lib.rs
+-rw-r--r--   0     1001      123     4967 2023-06-14 14:01:22.000000 opening_hours_py-0.6.7/src/types.rs
+-rw-r--r--   0     1001      123    29444 2023-06-14 14:01:22.000000 opening_hours_py-0.6.7/Cargo.lock
+-rw-r--r--   0        0        0     2344 1970-01-01 00:00:00.000000 opening_hours_py-0.6.7/PKG-INFO
```

### Comparing `opening_hours_py-0.6.6/local_dependencies/compact-calendar/Cargo.toml` & `opening_hours_py-0.6.7/local_dependencies/compact-calendar/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "compact-calendar"
-version = "0.6.6"
+version = "0.6.7"
 authors = ["Rémi Dupré <remi@dupre.io>"]
 license = "MIT OR Apache-2.0"
 readme = "README.md"
 repository = "https://github.com/remi-dupre/opening-hours-rs"
 documentation = "https://docs.rs/compact-calendar"
 homepage = "https://github.com/remi-dupre/opening-hours-rs/tree/master/compact-calendar"
 description = "Compact representation of a set of days based on a bit-maps"
```

### Comparing `opening_hours_py-0.6.6/local_dependencies/compact-calendar/README.md` & `opening_hours_py-0.6.7/local_dependencies/compact-calendar/README.md`

 * *Files identical despite different names*

### Comparing `opening_hours_py-0.6.6/local_dependencies/compact-calendar/src/lib.rs` & `opening_hours_py-0.6.7/local_dependencies/compact-calendar/src/lib.rs`

 * *Files identical despite different names*

### Comparing `opening_hours_py-0.6.6/local_dependencies/opening-hours/Cargo.toml` & `opening_hours_py-0.6.7/local_dependencies/opening-hours/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "opening-hours"
-version = "0.6.6"
+version = "0.6.7"
 authors = ["Rémi Dupré <remi@dupre.io>"]
 license = "MIT OR Apache-2.0"
 readme = "README.md"
 repository = "https://github.com/remi-dupre/opening-hours-rs"
 documentation = "https://docs.rs/opening-hours"
 homepage = "https://github.com/remi-dupre/opening-hours-rs"
 description = "A parser and evaluation tool for the opening_hours fields in OpenStreetMap."
```

### Comparing `opening_hours_py-0.6.6/local_dependencies/opening-hours/.github/workflows/deploy.yml` & `opening_hours_py-0.6.7/local_dependencies/opening-hours/.github/workflows/deploy.yml`

 * *Files 4% similar despite different names*

```diff
@@ -6,27 +6,28 @@
 env:
   CARGO_TERM_COLOR: always
 
 jobs:
   # ---
   # --- Check that all versions are consistency accross packages
   # ---
+
   check-version:
     runs-on: ubuntu-latest
 
     defaults:
       run:
         working-directory: scripts
 
     steps:
       - uses: actions/checkout@v2
 
       - uses: actions/setup-python@v2
         with:
-          python-version: "3.10"
+          python-version: "3.9"
 
       - name: Install poetry
         run: |
           python -m pip install --upgrade pip
           pip install poetry
 
       - name: Install dependancies
@@ -34,14 +35,15 @@
 
       - name: Check version consistency
         run: poetry run ./check-version.py
 
   # ---
   # --- Build an deploy Rust packages
   # ---
+
   deploy-rust:
     runs-on: ubuntu-latest
 
     strategy:
       max-parallel: 1
       matrix:
         crate:
@@ -71,17 +73,25 @@
       - name: Publish to crates.io
         run: cargo publish
         if: github.ref == 'refs/heads/master'
 
   # ---
   # --- Build and deploy Python bindings
   # ---
+
   deploy-python:
     runs-on: ubuntu-latest
 
+    strategy:
+      matrix:
+        python:
+          - "3.9"
+          - "3.10"
+          - "3.11"
+
     defaults:
       run:
         working-directory: python
 
     steps:
       - uses: actions/checkout@v2
 
@@ -89,15 +99,15 @@
         with:
           toolchain: stable
           default: true
           profile: minimal
 
       - uses: actions/setup-python@v2
         with:
-          python-version: "3.10"
+          python-version: ${{ matrix.python }}
 
       - name: Install poetry
         run: |
           python -m pip install --upgrade pip
           pip install poetry
 
       - name: Install dependancies
@@ -114,11 +124,11 @@
         if: github.ref == 'refs/heads/master'
         env:
           USER: remi-dupre
           PASS: ${{ secrets.PYPI_PASSWORD }}
 
       - name: Publish to github pages
         uses: peaceiris/actions-gh-pages@v3
-        if: github.ref == 'refs/heads/master'
+        if: github.ref == 'refs/heads/master' && matrix.python == '3.11'
         with:
           github_token: ${{ secrets.GITHUB_TOKEN }}
           publish_dir: ./python/docs
```

### Comparing `opening_hours_py-0.6.6/local_dependencies/opening-hours/.github/workflows/tests.yml` & `opening_hours_py-0.6.7/local_dependencies/opening-hours/.github/workflows/tests.yml`

 * *Files 0% similar despite different names*

```diff
@@ -67,15 +67,15 @@
         with:
           toolchain: stable
           default: true
           profile: minimal
 
       - uses: actions/setup-python@v2
         with:
-          python-version: "3.10"
+          python-version: "3.9"
 
       - name: Install poetry
         run: |
           python -m pip install --upgrade pip
           pip install poetry
 
       - name: Install dev dependancies
```

### Comparing `opening_hours_py-0.6.6/local_dependencies/opening-hours/Cargo.lock` & `opening_hours_py-0.6.7/local_dependencies/opening-hours/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -155,15 +155,15 @@
 name = "clap_lex"
 version = "0.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2da6da31387c7e4ef160ffab6d5e7f00c42626fe39aea70a7b0f1773f7dd6c1b"
 
 [[package]]
 name = "compact-calendar"
-version = "0.6.6"
+version = "0.6.7"
 dependencies = [
  "chrono",
 ]
 
 [[package]]
 name = "core-foundation-sys"
 version = "0.8.4"
@@ -537,37 +537,37 @@
 name = "oorandom"
 version = "11.1.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0ab1bc2a289d34bd04a330323ac98a1b4bc82c9d9fcb1e66b63caa84da26b575"
 
 [[package]]
 name = "opening-hours"
-version = "0.6.6"
+version = "0.6.7"
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
-version = "0.6.6"
+version = "0.6.7"
 dependencies = [
  "chrono",
  "opening-hours",
  "opening-hours-syntax",
  "pyo3",
 ]
 
 [[package]]
 name = "opening-hours-syntax"
-version = "0.6.6"
+version = "0.6.7"
 dependencies = [
  "chrono",
  "pest",
  "pest_derive",
 ]
 
 [[package]]
```

### Comparing `opening_hours_py-0.6.6/local_dependencies/opening-hours/LICENSE-APACHE` & `opening_hours_py-0.6.7/local_dependencies/opening-hours/LICENSE-APACHE`

 * *Files identical despite different names*

### Comparing `opening_hours_py-0.6.6/local_dependencies/opening-hours/LICENSE-MIT` & `opening_hours_py-0.6.7/local_dependencies/opening-hours/LICENSE-MIT`

 * *Files identical despite different names*

### Comparing `opening_hours_py-0.6.6/local_dependencies/opening-hours/README.md` & `opening_hours_py-0.6.7/local_dependencies/opening-hours/README.md`

 * *Files identical despite different names*

### Comparing `opening_hours_py-0.6.6/local_dependencies/opening-hours/benches/benchmarks.rs` & `opening_hours_py-0.6.7/local_dependencies/opening-hours/benches/benchmarks.rs`

 * *Files identical despite different names*

### Comparing `opening_hours_py-0.6.6/local_dependencies/opening-hours/build.rs` & `opening_hours_py-0.6.7/local_dependencies/opening-hours/build.rs`

 * *Files identical despite different names*

### Comparing `opening_hours_py-0.6.6/local_dependencies/opening-hours/data/holidays.txt` & `opening_hours_py-0.6.7/local_dependencies/opening-hours/data/holidays.txt`

 * *Files identical despite different names*

### Comparing `opening_hours_py-0.6.6/local_dependencies/opening-hours/scripts/check-version.py` & `opening_hours_py-0.6.7/local_dependencies/opening-hours/scripts/check-version.py`

 * *Files identical despite different names*

### Comparing `opening_hours_py-0.6.6/local_dependencies/opening-hours/scripts/generate-holidays.py` & `opening_hours_py-0.6.7/local_dependencies/opening-hours/scripts/generate-holidays.py`

 * *Files identical despite different names*

### Comparing `opening_hours_py-0.6.6/local_dependencies/opening-hours/scripts/poetry.lock` & `opening_hours_py-0.6.7/local_dependencies/opening-hours/scripts/poetry.lock`

 * *Files identical despite different names*

### Comparing `opening_hours_py-0.6.6/local_dependencies/opening-hours/src/bin/schedule.rs` & `opening_hours_py-0.6.7/local_dependencies/opening-hours/src/bin/schedule.rs`

 * *Files identical despite different names*

### Comparing `opening_hours_py-0.6.6/local_dependencies/opening-hours/src/date_filter.rs` & `opening_hours_py-0.6.7/local_dependencies/opening-hours/src/date_filter.rs`

 * *Files identical despite different names*

### Comparing `opening_hours_py-0.6.6/local_dependencies/opening-hours/src/opening_hours.rs` & `opening_hours_py-0.6.7/local_dependencies/opening-hours/src/opening_hours.rs`

 * *Files identical despite different names*

### Comparing `opening_hours_py-0.6.6/local_dependencies/opening-hours/src/schedule.rs` & `opening_hours_py-0.6.7/local_dependencies/opening-hours/src/schedule.rs`

 * *Files identical despite different names*

### Comparing `opening_hours_py-0.6.6/local_dependencies/opening-hours/src/tests/data/sample.txt` & `opening_hours_py-0.6.7/local_dependencies/opening-hours/src/tests/data/sample.txt`

 * *Files identical despite different names*

### Comparing `opening_hours_py-0.6.6/local_dependencies/opening-hours/src/tests/holiday_selector.rs` & `opening_hours_py-0.6.7/local_dependencies/opening-hours/src/tests/holiday_selector.rs`

 * *Files identical despite different names*

### Comparing `opening_hours_py-0.6.6/local_dependencies/opening-hours/src/tests/issues.rs` & `opening_hours_py-0.6.7/local_dependencies/opening-hours/src/tests/issues.rs`

 * *Files identical despite different names*

### Comparing `opening_hours_py-0.6.6/local_dependencies/opening-hours/src/tests/mod.rs` & `opening_hours_py-0.6.7/local_dependencies/opening-hours/src/tests/mod.rs`

 * *Files identical despite different names*

### Comparing `opening_hours_py-0.6.6/local_dependencies/opening-hours/src/tests/month_selector.rs` & `opening_hours_py-0.6.7/local_dependencies/opening-hours/src/tests/month_selector.rs`

 * *Files identical despite different names*

### Comparing `opening_hours_py-0.6.6/local_dependencies/opening-hours/src/tests/next_change.rs` & `opening_hours_py-0.6.7/local_dependencies/opening-hours/src/tests/next_change.rs`

 * *Files identical despite different names*

### Comparing `opening_hours_py-0.6.6/local_dependencies/opening-hours/src/tests/rules.rs` & `opening_hours_py-0.6.7/local_dependencies/opening-hours/src/tests/rules.rs`

 * *Files identical despite different names*

### Comparing `opening_hours_py-0.6.6/local_dependencies/opening-hours/src/tests/selective.rs` & `opening_hours_py-0.6.7/local_dependencies/opening-hours/src/tests/selective.rs`

 * *Files identical despite different names*

### Comparing `opening_hours_py-0.6.6/local_dependencies/opening-hours/src/tests/time_selector.rs` & `opening_hours_py-0.6.7/local_dependencies/opening-hours/src/tests/time_selector.rs`

 * *Files identical despite different names*

### Comparing `opening_hours_py-0.6.6/local_dependencies/opening-hours/src/tests/week_selector.rs` & `opening_hours_py-0.6.7/local_dependencies/opening-hours/src/tests/week_selector.rs`

 * *Files identical despite different names*

### Comparing `opening_hours_py-0.6.6/local_dependencies/opening-hours/src/tests/weekday_selector.rs` & `opening_hours_py-0.6.7/local_dependencies/opening-hours/src/tests/weekday_selector.rs`

 * *Files identical despite different names*

### Comparing `opening_hours_py-0.6.6/local_dependencies/opening-hours/src/tests/year_selector.rs` & `opening_hours_py-0.6.7/local_dependencies/opening-hours/src/tests/year_selector.rs`

 * *Files identical despite different names*

### Comparing `opening_hours_py-0.6.6/local_dependencies/opening-hours/src/time_filter.rs` & `opening_hours_py-0.6.7/local_dependencies/opening-hours/src/time_filter.rs`

 * *Files identical despite different names*

### Comparing `opening_hours_py-0.6.6/local_dependencies/opening-hours/src/utils/range.rs` & `opening_hours_py-0.6.7/local_dependencies/opening-hours/src/utils/range.rs`

 * *Files identical despite different names*

### Comparing `opening_hours_py-0.6.6/local_dependencies/opening-hours-syntax/Cargo.toml` & `opening_hours_py-0.6.7/local_dependencies/opening-hours-syntax/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "opening-hours-syntax"
-version = "0.6.6"
+version = "0.6.7"
 authors = ["Rémi Dupré <remi@dupre.io>"]
 license = "MIT OR Apache-2.0"
 readme = "README.md"
 repository = "https://github.com/remi-dupre/opening-hours-rs"
 documentation = "https://docs.rs/opening-hours-syntax"
 homepage = "https://github.com/remi-dupre/opening-hours-rs/tree/master/opening-hours-syntax"
 description = "A parser for opening_hours fields in OpenStreetMap."
```

### Comparing `opening_hours_py-0.6.6/local_dependencies/opening-hours-syntax/LICENSE-APACHE` & `opening_hours_py-0.6.7/local_dependencies/opening-hours-syntax/LICENSE-APACHE`

 * *Files identical despite different names*

### Comparing `opening_hours_py-0.6.6/local_dependencies/opening-hours-syntax/LICENSE-MIT` & `opening_hours_py-0.6.7/local_dependencies/opening-hours-syntax/LICENSE-MIT`

 * *Files identical despite different names*

### Comparing `opening_hours_py-0.6.6/local_dependencies/opening-hours-syntax/README.md` & `opening_hours_py-0.6.7/local_dependencies/opening-hours-syntax/README.md`

 * *Files identical despite different names*

### Comparing `opening_hours_py-0.6.6/local_dependencies/opening-hours-syntax/src/error.rs` & `opening_hours_py-0.6.7/local_dependencies/opening-hours-syntax/src/error.rs`

 * *Files identical despite different names*

### Comparing `opening_hours_py-0.6.6/local_dependencies/opening-hours-syntax/src/extended_time.rs` & `opening_hours_py-0.6.7/local_dependencies/opening-hours-syntax/src/extended_time.rs`

 * *Files identical despite different names*

### Comparing `opening_hours_py-0.6.6/local_dependencies/opening-hours-syntax/src/grammar.pest` & `opening_hours_py-0.6.7/local_dependencies/opening-hours-syntax/src/grammar.pest`

 * *Files identical despite different names*

### Comparing `opening_hours_py-0.6.6/local_dependencies/opening-hours-syntax/src/lib.rs` & `opening_hours_py-0.6.7/local_dependencies/opening-hours-syntax/src/lib.rs`

 * *Files identical despite different names*

### Comparing `opening_hours_py-0.6.6/local_dependencies/opening-hours-syntax/src/parser.rs` & `opening_hours_py-0.6.7/local_dependencies/opening-hours-syntax/src/parser.rs`

 * *Files identical despite different names*

### Comparing `opening_hours_py-0.6.6/local_dependencies/opening-hours-syntax/src/rules/day.rs` & `opening_hours_py-0.6.7/local_dependencies/opening-hours-syntax/src/rules/day.rs`

 * *Files identical despite different names*

### Comparing `opening_hours_py-0.6.6/local_dependencies/opening-hours-syntax/src/rules/mod.rs` & `opening_hours_py-0.6.7/local_dependencies/opening-hours-syntax/src/rules/mod.rs`

 * *Files identical despite different names*

### Comparing `opening_hours_py-0.6.6/local_dependencies/opening-hours-syntax/src/rules/time.rs` & `opening_hours_py-0.6.7/local_dependencies/opening-hours-syntax/src/rules/time.rs`

 * *Files identical despite different names*

### Comparing `opening_hours_py-0.6.6/local_dependencies/opening-hours-syntax/src/sorted_vec.rs` & `opening_hours_py-0.6.7/local_dependencies/opening-hours-syntax/src/sorted_vec.rs`

 * *Files identical despite different names*

### Comparing `opening_hours_py-0.6.6/Cargo.toml` & `opening_hours_py-0.6.7/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "opening-hours-py"
-version = "0.6.6"
+version = "0.6.7"
 authors = ["Rémi Dupré <remi@dupre.io>"]
 license = "MIT OR Apache-2.0"
 readme = "README.md"
 repository = "https://github.com/remi-dupre/opening-hours-rs"
 documentation = "https://remi-dupre.github.io/opening-hours-rs/opening_hours.html"
 homepage = "https://github.com/remi-dupre/opening-hours-rs/tree/master/python"
 description = "A parser and toolkit for the opening_hours in OpenStreetMap written in Rust."
```

### Comparing `opening_hours_py-0.6.6/LICENSE-APACHE` & `opening_hours_py-0.6.7/LICENSE-APACHE`

 * *Files identical despite different names*

### Comparing `opening_hours_py-0.6.6/LICENSE-MIT` & `opening_hours_py-0.6.7/LICENSE-MIT`

 * *Files identical despite different names*

### Comparing `opening_hours_py-0.6.6/README.md` & `opening_hours_py-0.6.7/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,17 @@
 [![PyPI](https://img.shields.io/pypi/v/opening-hours-py)](https://pypi.org/project/opening-hours-py/)
 [![Doc](https://img.shields.io/badge/doc-pdoc-blue)](https://remi-dupre.github.io/opening-hours-rs/opening_hours.html)
 
 
 Usage
 -----
 
+The package is published for Python 3.9 and above, but you should be able to install it
+with older version of python if you install the Rust toolchain.
+
 Install `opening-hours-py` from PyPI, for example using pip:
 
 ```bash
 pip install --user opening-hours-py
 ```
 
 Then, the main object that you will interact with will be `OpeningHours`:
```

### Comparing `opening_hours_py-0.6.6/poetry.lock` & `opening_hours_py-0.6.7/poetry.lock`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,25 @@
 # This file is automatically @generated by Poetry 1.5.1 and should not be changed by hand.
 
 [[package]]
+name = "astunparse"
+version = "1.6.3"
+description = "An AST unparser for Python"
+optional = false
+python-versions = "*"
+files = [
+    {file = "astunparse-1.6.3-py2.py3-none-any.whl", hash = "sha256:c2652417f2c8b5bb325c885ae329bdf3f86424075c4fd1a128674bc6fba4b8e8"},
+    {file = "astunparse-1.6.3.tar.gz", hash = "sha256:5ad93a8456f0d084c3456d059fd9a92cce667963232cbf763eac3bc5b7940872"},
+]
+
+[package.dependencies]
+six = ">=1.6.1,<2.0"
+wheel = ">=0.23.0,<1.0"
+
+[[package]]
 name = "jinja2"
 version = "3.1.2"
 description = "A very fast and expressive template engine."
 optional = false
 python-versions = ">=3.7"
 files = [
     {file = "Jinja2-3.1.2-py3-none-any.whl", hash = "sha256:6088930bfe239f0e6710546ab9c19c9ef35e29792895fed6e6e31a023a182a61"},
@@ -113,14 +128,15 @@
 python-versions = ">=3.7"
 files = [
     {file = "pdoc-12.3.1-py3-none-any.whl", hash = "sha256:c3f24f31286e634de9c76fa6e67bd5c0c5e74360b41dc91e6b82499831eb52d8"},
     {file = "pdoc-12.3.1.tar.gz", hash = "sha256:453236f225feddb8a9071428f1982a78d74b9b3da4bc4433aedb64dbd0cc87ab"},
 ]
 
 [package.dependencies]
+astunparse = {version = "*", markers = "python_version < \"3.9\""}
 Jinja2 = ">=2.11.0"
 MarkupSafe = "*"
 pygments = ">=2.12.0"
 
 [package.extras]
 dev = ["black", "hypothesis", "mypy", "pytest", "pytest-cov", "pytest-timeout", "ruff", "tox", "types-pygments"]
 
@@ -135,21 +151,46 @@
     {file = "Pygments-2.15.1.tar.gz", hash = "sha256:8ace4d3c1dd481894b2005f560ead0f9f19ee64fe983366be1a21e171d12775c"},
 ]
 
 [package.extras]
 plugins = ["importlib-metadata"]
 
 [[package]]
+name = "six"
+version = "1.16.0"
+description = "Python 2 and 3 compatibility utilities"
+optional = false
+python-versions = ">=2.7, !=3.0.*, !=3.1.*, !=3.2.*"
+files = [
+    {file = "six-1.16.0-py2.py3-none-any.whl", hash = "sha256:8abb2f1d86890a2dfb989f9a77cfcfd3e47c2a354b01111771326f8aa26e0254"},
+    {file = "six-1.16.0.tar.gz", hash = "sha256:1e61c37477a1626458e36f7b1d82aa5c9b094fa4802892072e49de9c60c4c926"},
+]
+
+[[package]]
 name = "tomli"
 version = "2.0.1"
 description = "A lil' TOML parser"
 optional = false
 python-versions = ">=3.7"
 files = [
     {file = "tomli-2.0.1-py3-none-any.whl", hash = "sha256:939de3e7a6161af0c887ef91b7d41a53e7c5a1ca976325f429cb46ea9bc30ecc"},
     {file = "tomli-2.0.1.tar.gz", hash = "sha256:de526c12914f0c550d15924c62d72abc48d6fe7364aa87328337a31007fe8a4f"},
 ]
 
+[[package]]
+name = "wheel"
+version = "0.40.0"
+description = "A built-package format for Python"
+optional = false
+python-versions = ">=3.7"
+files = [
+    {file = "wheel-0.40.0-py3-none-any.whl", hash = "sha256:d236b20e7cb522daf2390fa84c55eea81c5c30190f90f29ae2ca1ad8355bf247"},
+    {file = "wheel-0.40.0.tar.gz", hash = "sha256:cd1196f3faee2b31968d626e1731c94f99cbdb67cf5a46e4f5656cbee7738873"},
+]
+
+[package.extras]
+test = ["pytest (>=6.0.0)"]
+
 [metadata]
 lock-version = "2.0"
-python-versions = "^3.9"
-content-hash = "332291e13df8556b5ef6194f642affff2f47b0b4e160db01447c3a9e3039ae00"
+python-versions = "^3.8"
+content-hash = "217c1268eb52923df9488713fdd4cedd827a865ac7151202cbaa6bf3de881d62"
```

### Comparing `opening_hours_py-0.6.6/src/errors.rs` & `opening_hours_py-0.6.7/src/errors.rs`

 * *Files identical despite different names*

### Comparing `opening_hours_py-0.6.6/src/lib.rs` & `opening_hours_py-0.6.7/src/lib.rs`

 * *Files identical despite different names*

### Comparing `opening_hours_py-0.6.6/src/types.rs` & `opening_hours_py-0.6.7/src/types.rs`

 * *Files identical despite different names*

### Comparing `opening_hours_py-0.6.6/Cargo.lock` & `opening_hours_py-0.6.7/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -155,15 +155,15 @@
 name = "clap_lex"
 version = "0.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2da6da31387c7e4ef160ffab6d5e7f00c42626fe39aea70a7b0f1773f7dd6c1b"
 
 [[package]]
 name = "compact-calendar"
-version = "0.6.6"
+version = "0.6.7"
 dependencies = [
  "chrono",
 ]
 
 [[package]]
 name = "core-foundation-sys"
 version = "0.8.4"
@@ -537,37 +537,37 @@
 name = "oorandom"
 version = "11.1.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0ab1bc2a289d34bd04a330323ac98a1b4bc82c9d9fcb1e66b63caa84da26b575"
 
 [[package]]
 name = "opening-hours"
-version = "0.6.6"
+version = "0.6.7"
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
-version = "0.6.6"
+version = "0.6.7"
 dependencies = [
  "chrono",
  "opening-hours",
  "opening-hours-syntax",
  "pyo3",
 ]
 
 [[package]]
 name = "opening-hours-syntax"
-version = "0.6.6"
+version = "0.6.7"
 dependencies = [
  "chrono",
  "pest",
  "pest_derive",
 ]
 
 [[package]]
```

### Comparing `opening_hours_py-0.6.6/PKG-INFO` & `opening_hours_py-0.6.7/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opening-hours-py
-Version: 0.6.6
+Version: 0.6.7
 Summary: A parser and toolkit for the opening_hours in OpenStreetMap written in Rust.
 Home-Page: https://github.com/remi-dupre/opening-hours-rs/tree/master/python
 Author: Rémi Dupré <remi@dupre.io>
 Author-email: Rémi Dupré <remi@dupre.io>
 License: MIT OR Apache-2.0
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 Project-URL: Source Code, https://github.com/remi-dupre/opening-hours-rs
@@ -15,14 +15,17 @@
 [![PyPI](https://img.shields.io/pypi/v/opening-hours-py)](https://pypi.org/project/opening-hours-py/)
 [![Doc](https://img.shields.io/badge/doc-pdoc-blue)](https://remi-dupre.github.io/opening-hours-rs/opening_hours.html)
 
 
 Usage
 -----
 
+The package is published for Python 3.9 and above, but you should be able to install it
+with older version of python if you install the Rust toolchain.
+
 Install `opening-hours-py` from PyPI, for example using pip:
 
 ```bash
 pip install --user opening-hours-py
 ```
 
 Then, the main object that you will interact with will be `OpeningHours`:
```

