# Comparing `tmp/rithm-9.3.0.tar.gz` & `tmp/rithm-9.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rithm-9.3.0.tar", last modified: Sun Jun 19 15:53:31 2022, max compression
+gzip compressed data, was "rithm-9.4.0.tar", last modified: Mon Jun 20 07:52:58 2022, max compression
```

## Comparing `rithm-9.3.0.tar` & `rithm-9.4.0.tar`

### file list

```diff
@@ -1,129 +1,129 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-19 15:53:31.405501 rithm-9.3.0/
--rw-r--r--   0 runner    (1001) docker     (121)      405 2022-06-19 15:53:15.000000 rithm-9.3.0/Cargo.toml
--rw-r--r--   0 runner    (1001) docker     (121)     1069 2022-06-19 15:53:15.000000 rithm-9.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       93 2022-06-19 15:53:15.000000 rithm-9.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)    10214 2022-06-19 15:53:31.405501 rithm-9.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     9448 2022-06-19 15:53:15.000000 rithm-9.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       71 2022-06-19 15:53:15.000000 rithm-9.3.0/requirements-setup.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-19 15:53:31.393501 rithm-9.3.0/rithm/
--rw-r--r--   0 runner    (1001) docker     (121)      371 2022-06-19 15:53:15.000000 rithm-9.3.0/rithm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7586 2022-06-19 15:53:15.000000 rithm-9.3.0/rithm/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)    24937 2022-06-19 15:53:15.000000 rithm-9.3.0/rithm/_rithm.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-19 15:53:15.000000 rithm-9.3.0/rithm/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-19 15:53:31.393501 rithm-9.3.0/rithm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    10214 2022-06-19 15:53:30.000000 rithm-9.3.0/rithm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2894 2022-06-19 15:53:31.000000 rithm-9.3.0/rithm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-19 15:53:30.000000 rithm-9.3.0/rithm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-19 15:53:30.000000 rithm-9.3.0/rithm.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-06-19 15:53:31.000000 rithm-9.3.0/rithm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-06-19 15:53:31.405501 rithm-9.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2025 2022-06-19 15:53:15.000000 rithm-9.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-19 15:53:31.393501 rithm-9.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-19 15:53:31.397501 rithm-9.3.0/src/big_int/
--rw-r--r--   0 runner    (1001) docker     (121)      632 2022-06-19 15:53:15.000000 rithm-9.3.0/src/big_int/abs.rs
--rw-r--r--   0 runner    (1001) docker     (121)     1666 2022-06-19 15:53:15.000000 rithm-9.3.0/src/big_int/add.rs
--rw-r--r--   0 runner    (1001) docker     (121)      724 2022-06-19 15:53:15.000000 rithm-9.3.0/src/big_int/add_assign.rs
--rw-r--r--   0 runner    (1001) docker     (121)     1995 2022-06-19 15:53:15.000000 rithm-9.3.0/src/big_int/bit_and.rs
--rw-r--r--   0 runner    (1001) docker     (121)      907 2022-06-19 15:53:15.000000 rithm-9.3.0/src/big_int/bit_and_assign.rs
--rw-r--r--   0 runner    (1001) docker     (121)      825 2022-06-19 15:53:15.000000 rithm-9.3.0/src/big_int/bit_length.rs
--rw-r--r--   0 runner    (1001) docker     (121)     1934 2022-06-19 15:53:15.000000 rithm-9.3.0/src/big_int/bit_or.rs
--rw-r--r--   0 runner    (1001) docker     (121)      899 2022-06-19 15:53:15.000000 rithm-9.3.0/src/big_int/bit_or_assign.rs
--rw-r--r--   0 runner    (1001) docker     (121)     2040 2022-06-19 15:53:15.000000 rithm-9.3.0/src/big_int/bit_xor.rs
--rw-r--r--   0 runner    (1001) docker     (121)      934 2022-06-19 15:53:15.000000 rithm-9.3.0/src/big_int/bit_xor_assign.rs
--rw-r--r--   0 runner    (1001) docker     (121)     1782 2022-06-19 15:53:15.000000 rithm-9.3.0/src/big_int/checked_div.rs
--rw-r--r--   0 runner    (1001) docker     (121)     1929 2022-06-19 15:53:15.000000 rithm-9.3.0/src/big_int/checked_div_as_f32.rs
--rw-r--r--   0 runner    (1001) docker     (121)     1929 2022-06-19 15:53:15.000000 rithm-9.3.0/src/big_int/checked_div_as_f64.rs
--rw-r--r--   0 runner    (1001) docker     (121)     1905 2022-06-19 15:53:15.000000 rithm-9.3.0/src/big_int/checked_div_euclid.rs
--rw-r--r--   0 runner    (1001) docker     (121)     3551 2022-06-19 15:53:15.000000 rithm-9.3.0/src/big_int/checked_div_rem.rs
--rw-r--r--   0 runner    (1001) docker     (121)     3946 2022-06-19 15:53:15.000000 rithm-9.3.0/src/big_int/checked_div_rem_euclid.rs
--rw-r--r--   0 runner    (1001) docker     (121)     4556 2022-06-19 15:53:15.000000 rithm-9.3.0/src/big_int/checked_pow.rs
--rw-r--r--   0 runner    (1001) docker     (121)    12701 2022-06-19 15:53:15.000000 rithm-9.3.0/src/big_int/checked_pow_rem_euclid.rs
--rw-r--r--   0 runner    (1001) docker     (121)     1782 2022-06-19 15:53:15.000000 rithm-9.3.0/src/big_int/checked_rem.rs
--rw-r--r--   0 runner    (1001) docker     (121)     1905 2022-06-19 15:53:15.000000 rithm-9.3.0/src/big_int/checked_rem_euclid.rs
--rw-r--r--   0 runner    (1001) docker     (121)     2209 2022-06-19 15:53:15.000000 rithm-9.3.0/src/big_int/checked_rem_euclid_inv.rs
--rw-r--r--   0 runner    (1001) docker     (121)     5736 2022-06-19 15:53:15.000000 rithm-9.3.0/src/big_int/checked_shl.rs
--rw-r--r--   0 runner    (1001) docker     (121)     6324 2022-06-19 15:53:15.000000 rithm-9.3.0/src/big_int/checked_shr.rs
--rw-r--r--   0 runner    (1001) docker     (121)      299 2022-06-19 15:53:15.000000 rithm-9.3.0/src/big_int/constants.rs
--rw-r--r--   0 runner    (1001) docker     (121)      278 2022-06-19 15:53:15.000000 rithm-9.3.0/src/big_int/contracts.rs
--rw-r--r--   0 runner    (1001) docker     (121)    74998 2022-06-19 15:53:15.000000 rithm-9.3.0/src/big_int/digits.rs
--rw-r--r--   0 runner    (1001) docker     (121)     3129 2022-06-19 15:53:15.000000 rithm-9.3.0/src/big_int/display.rs
--rw-r--r--   0 runner    (1001) docker     (121)     2222 2022-06-19 15:53:15.000000 rithm-9.3.0/src/big_int/div.rs
--rw-r--r--   0 runner    (1001) docker     (121)      903 2022-06-19 15:53:15.000000 rithm-9.3.0/src/big_int/div_assign.rs
--rw-r--r--   0 runner    (1001) docker     (121)     2252 2022-06-19 15:53:15.000000 rithm-9.3.0/src/big_int/div_euclid.rs
--rw-r--r--   0 runner    (1001) docker     (121)     1618 2022-06-19 15:53:15.000000 rithm-9.3.0/src/big_int/div_rem.rs
--rw-r--r--   0 runner    (1001) docker     (121)     1740 2022-06-19 15:53:15.000000 rithm-9.3.0/src/big_int/div_rem_euclid.rs
--rw-r--r--   0 runner    (1001) docker     (121)      708 2022-06-19 15:53:15.000000 rithm-9.3.0/src/big_int/float_to_int.rs
--rw-r--r--   0 runner    (1001) docker     (121)      821 2022-06-19 15:53:15.000000 rithm-9.3.0/src/big_int/from.rs
--rw-r--r--   0 runner    (1001) docker     (121)     1315 2022-06-19 15:53:15.000000 rithm-9.3.0/src/big_int/from_bytes.rs
--rw-r--r--   0 runner    (1001) docker     (121)      711 2022-06-19 15:53:15.000000 rithm-9.3.0/src/big_int/from_str_radix.rs
--rw-r--r--   0 runner    (1001) docker     (121)     1490 2022-06-19 15:53:15.000000 rithm-9.3.0/src/big_int/gcd.rs
--rw-r--r--   0 runner    (1001) docker     (121)      286 2022-06-19 15:53:15.000000 rithm-9.3.0/src/big_int/hash.rs
--rw-r--r--   0 runner    (1001) docker     (121)      478 2022-06-19 15:53:15.000000 rithm-9.3.0/src/big_int/is_power_of_two.rs
--rw-r--r--   0 runner    (1001) docker     (121)     1071 2022-06-19 15:53:15.000000 rithm-9.3.0/src/big_int/mod.rs
--rw-r--r--   0 runner    (1001) docker     (121)     1673 2022-06-19 15:53:15.000000 rithm-9.3.0/src/big_int/mul.rs
--rw-r--r--   0 runner    (1001) docker     (121)      715 2022-06-19 15:53:15.000000 rithm-9.3.0/src/big_int/mul_assign.rs
--rw-r--r--   0 runner    (1001) docker     (121)      617 2022-06-19 15:53:15.000000 rithm-9.3.0/src/big_int/neg.rs
--rw-r--r--   0 runner    (1001) docker     (121)      751 2022-06-19 15:53:15.000000 rithm-9.3.0/src/big_int/not.rs
--rw-r--r--   0 runner    (1001) docker     (121)      448 2022-06-19 15:53:15.000000 rithm-9.3.0/src/big_int/ord.rs
--rw-r--r--   0 runner    (1001) docker     (121)      391 2022-06-19 15:53:15.000000 rithm-9.3.0/src/big_int/parity.rs
--rw-r--r--   0 runner    (1001) docker     (121)     1272 2022-06-19 15:53:15.000000 rithm-9.3.0/src/big_int/partial_eq.rs
--rw-r--r--   0 runner    (1001) docker     (121)    14595 2022-06-19 15:53:15.000000 rithm-9.3.0/src/big_int/partial_ord.rs
--rw-r--r--   0 runner    (1001) docker     (121)     1422 2022-06-19 15:53:15.000000 rithm-9.3.0/src/big_int/pow.rs
--rw-r--r--   0 runner    (1001) docker     (121)     1997 2022-06-19 15:53:15.000000 rithm-9.3.0/src/big_int/rem.rs
--rw-r--r--   0 runner    (1001) docker     (121)      903 2022-06-19 15:53:15.000000 rithm-9.3.0/src/big_int/rem_assign.rs
--rw-r--r--   0 runner    (1001) docker     (121)     2252 2022-06-19 15:53:15.000000 rithm-9.3.0/src/big_int/rem_euclid.rs
--rw-r--r--   0 runner    (1001) docker     (121)      332 2022-06-19 15:53:15.000000 rithm-9.3.0/src/big_int/signed.rs
--rw-r--r--   0 runner    (1001) docker     (121)     1939 2022-06-19 15:53:15.000000 rithm-9.3.0/src/big_int/sub.rs
--rw-r--r--   0 runner    (1001) docker     (121)      863 2022-06-19 15:53:15.000000 rithm-9.3.0/src/big_int/sub_assign.rs
--rw-r--r--   0 runner    (1001) docker     (121)     1405 2022-06-19 15:53:15.000000 rithm-9.3.0/src/big_int/to_bytes.rs
--rw-r--r--   0 runner    (1001) docker     (121)     1682 2022-06-19 15:53:15.000000 rithm-9.3.0/src/big_int/try_from.rs
--rw-r--r--   0 runner    (1001) docker     (121)     5116 2022-06-19 15:53:15.000000 rithm-9.3.0/src/big_int/try_from_string.rs
--rw-r--r--   0 runner    (1001) docker     (121)     4703 2022-06-19 15:53:15.000000 rithm-9.3.0/src/big_int/try_into.rs
--rw-r--r--   0 runner    (1001) docker     (121)     7774 2022-06-19 15:53:15.000000 rithm-9.3.0/src/big_int/types.rs
--rw-r--r--   0 runner    (1001) docker     (121)      428 2022-06-19 15:53:15.000000 rithm-9.3.0/src/big_int/unitary.rs
--rw-r--r--   0 runner    (1001) docker     (121)      378 2022-06-19 15:53:15.000000 rithm-9.3.0/src/big_int/zeroable.rs
--rw-r--r--   0 runner    (1001) docker     (121)       92 2022-06-19 15:53:15.000000 rithm-9.3.0/src/constants.rs
--rw-r--r--   0 runner    (1001) docker     (121)      520 2022-06-19 15:53:15.000000 rithm-9.3.0/src/contracts.rs
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-19 15:53:31.405501 rithm-9.3.0/src/fraction/
--rw-r--r--   0 runner    (1001) docker     (121)      350 2022-06-19 15:53:15.000000 rithm-9.3.0/src/fraction/abs.rs
--rw-r--r--   0 runner    (1001) docker     (121)     1931 2022-06-19 15:53:15.000000 rithm-9.3.0/src/fraction/add.rs
--rw-r--r--   0 runner    (1001) docker     (121)     1083 2022-06-19 15:53:15.000000 rithm-9.3.0/src/fraction/add_assign.rs
--rw-r--r--   0 runner    (1001) docker     (121)      581 2022-06-19 15:53:15.000000 rithm-9.3.0/src/fraction/ceil.rs
--rw-r--r--   0 runner    (1001) docker     (121)     3137 2022-06-19 15:53:15.000000 rithm-9.3.0/src/fraction/checked_div.rs
--rw-r--r--   0 runner    (1001) docker     (121)     1765 2022-06-19 15:53:15.000000 rithm-9.3.0/src/fraction/checked_div_euclid.rs
--rw-r--r--   0 runner    (1001) docker     (121)     3845 2022-06-19 15:53:15.000000 rithm-9.3.0/src/fraction/checked_div_rem_euclid.rs
--rw-r--r--   0 runner    (1001) docker     (121)     1795 2022-06-19 15:53:15.000000 rithm-9.3.0/src/fraction/checked_pow.rs
--rw-r--r--   0 runner    (1001) docker     (121)     3147 2022-06-19 15:53:15.000000 rithm-9.3.0/src/fraction/checked_rem.rs
--rw-r--r--   0 runner    (1001) docker     (121)     3307 2022-06-19 15:53:15.000000 rithm-9.3.0/src/fraction/checked_rem_euclid.rs
--rw-r--r--   0 runner    (1001) docker     (121)      701 2022-06-19 15:53:15.000000 rithm-9.3.0/src/fraction/debug.rs
--rw-r--r--   0 runner    (1001) docker     (121)      438 2022-06-19 15:53:15.000000 rithm-9.3.0/src/fraction/display.rs
--rw-r--r--   0 runner    (1001) docker     (121)     1661 2022-06-19 15:53:15.000000 rithm-9.3.0/src/fraction/div.rs
--rw-r--r--   0 runner    (1001) docker     (121)     1247 2022-06-19 15:53:15.000000 rithm-9.3.0/src/fraction/div_assign.rs
--rw-r--r--   0 runner    (1001) docker     (121)     1977 2022-06-19 15:53:15.000000 rithm-9.3.0/src/fraction/div_euclid.rs
--rw-r--r--   0 runner    (1001) docker     (121)       87 2022-06-19 15:53:15.000000 rithm-9.3.0/src/fraction/eq.rs
--rw-r--r--   0 runner    (1001) docker     (121)      478 2022-06-19 15:53:15.000000 rithm-9.3.0/src/fraction/floor.rs
--rw-r--r--   0 runner    (1001) docker     (121)      279 2022-06-19 15:53:15.000000 rithm-9.3.0/src/fraction/from.rs
--rw-r--r--   0 runner    (1001) docker     (121)      251 2022-06-19 15:53:15.000000 rithm-9.3.0/src/fraction/hash.rs
--rw-r--r--   0 runner    (1001) docker     (121)      541 2022-06-19 15:53:15.000000 rithm-9.3.0/src/fraction/mod.rs
--rw-r--r--   0 runner    (1001) docker     (121)     1816 2022-06-19 15:53:15.000000 rithm-9.3.0/src/fraction/mul.rs
--rw-r--r--   0 runner    (1001) docker     (121)     1115 2022-06-19 15:53:15.000000 rithm-9.3.0/src/fraction/mul_assign.rs
--rw-r--r--   0 runner    (1001) docker     (121)      362 2022-06-19 15:53:15.000000 rithm-9.3.0/src/fraction/neg.rs
--rw-r--r--   0 runner    (1001) docker     (121)      419 2022-06-19 15:53:15.000000 rithm-9.3.0/src/fraction/ord.rs
--rw-r--r--   0 runner    (1001) docker     (121)     1224 2022-06-19 15:53:15.000000 rithm-9.3.0/src/fraction/partial_eq.rs
--rw-r--r--   0 runner    (1001) docker     (121)     3995 2022-06-19 15:53:15.000000 rithm-9.3.0/src/fraction/partial_ord.rs
--rw-r--r--   0 runner    (1001) docker     (121)      986 2022-06-19 15:53:15.000000 rithm-9.3.0/src/fraction/pow.rs
--rw-r--r--   0 runner    (1001) docker     (121)     1885 2022-06-19 15:53:15.000000 rithm-9.3.0/src/fraction/rem.rs
--rw-r--r--   0 runner    (1001) docker     (121)     1490 2022-06-19 15:53:15.000000 rithm-9.3.0/src/fraction/rem_assign.rs
--rw-r--r--   0 runner    (1001) docker     (121)     1987 2022-06-19 15:53:15.000000 rithm-9.3.0/src/fraction/rem_euclid.rs
--rw-r--r--   0 runner    (1001) docker     (121)     1492 2022-06-19 15:53:15.000000 rithm-9.3.0/src/fraction/round.rs
--rw-r--r--   0 runner    (1001) docker     (121)      304 2022-06-19 15:53:15.000000 rithm-9.3.0/src/fraction/signed.rs
--rw-r--r--   0 runner    (1001) docker     (121)     2595 2022-06-19 15:53:15.000000 rithm-9.3.0/src/fraction/sub.rs
--rw-r--r--   0 runner    (1001) docker     (121)     1126 2022-06-19 15:53:15.000000 rithm-9.3.0/src/fraction/sub_assign.rs
--rw-r--r--   0 runner    (1001) docker     (121)      451 2022-06-19 15:53:15.000000 rithm-9.3.0/src/fraction/trunc.rs
--rw-r--r--   0 runner    (1001) docker     (121)     4719 2022-06-19 15:53:15.000000 rithm-9.3.0/src/fraction/try_from.rs
--rw-r--r--   0 runner    (1001) docker     (121)      987 2022-06-19 15:53:15.000000 rithm-9.3.0/src/fraction/try_into.rs
--rw-r--r--   0 runner    (1001) docker     (121)     2378 2022-06-19 15:53:15.000000 rithm-9.3.0/src/fraction/types.rs
--rw-r--r--   0 runner    (1001) docker     (121)      364 2022-06-19 15:53:15.000000 rithm-9.3.0/src/fraction/unitary.rs
--rw-r--r--   0 runner    (1001) docker     (121)      363 2022-06-19 15:53:15.000000 rithm-9.3.0/src/fraction/zero.rs
--rw-r--r--   0 runner    (1001) docker     (121)    43036 2022-06-19 15:53:15.000000 rithm-9.3.0/src/lib.rs
--rw-r--r--   0 runner    (1001) docker     (121)    39513 2022-06-19 15:53:15.000000 rithm-9.3.0/src/traits.rs
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-20 07:52:58.120713 rithm-9.4.0/
+-rw-r--r--   0 runner    (1001) docker     (121)      405 2022-06-20 07:52:36.000000 rithm-9.4.0/Cargo.toml
+-rw-r--r--   0 runner    (1001) docker     (121)     1069 2022-06-20 07:52:36.000000 rithm-9.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)       93 2022-06-20 07:52:36.000000 rithm-9.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)    10214 2022-06-20 07:52:58.120713 rithm-9.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     9448 2022-06-20 07:52:36.000000 rithm-9.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)       71 2022-06-20 07:52:36.000000 rithm-9.4.0/requirements-setup.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-20 07:52:58.100712 rithm-9.4.0/rithm/
+-rw-r--r--   0 runner    (1001) docker     (121)      371 2022-06-20 07:52:36.000000 rithm-9.4.0/rithm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7586 2022-06-20 07:52:36.000000 rithm-9.4.0/rithm/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)    24937 2022-06-20 07:52:36.000000 rithm-9.4.0/rithm/_rithm.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-20 07:52:36.000000 rithm-9.4.0/rithm/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-20 07:52:58.100712 rithm-9.4.0/rithm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)    10214 2022-06-20 07:52:57.000000 rithm-9.4.0/rithm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2894 2022-06-20 07:52:58.000000 rithm-9.4.0/rithm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-20 07:52:57.000000 rithm-9.4.0/rithm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-20 07:52:57.000000 rithm-9.4.0/rithm.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)        6 2022-06-20 07:52:57.000000 rithm-9.4.0/rithm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-06-20 07:52:58.120713 rithm-9.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     2025 2022-06-20 07:52:36.000000 rithm-9.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-20 07:52:58.100712 rithm-9.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-20 07:52:58.112712 rithm-9.4.0/src/big_int/
+-rw-r--r--   0 runner    (1001) docker     (121)      632 2022-06-20 07:52:36.000000 rithm-9.4.0/src/big_int/abs.rs
+-rw-r--r--   0 runner    (1001) docker     (121)     1666 2022-06-20 07:52:36.000000 rithm-9.4.0/src/big_int/add.rs
+-rw-r--r--   0 runner    (1001) docker     (121)      724 2022-06-20 07:52:36.000000 rithm-9.4.0/src/big_int/add_assign.rs
+-rw-r--r--   0 runner    (1001) docker     (121)     1995 2022-06-20 07:52:36.000000 rithm-9.4.0/src/big_int/bit_and.rs
+-rw-r--r--   0 runner    (1001) docker     (121)      907 2022-06-20 07:52:36.000000 rithm-9.4.0/src/big_int/bit_and_assign.rs
+-rw-r--r--   0 runner    (1001) docker     (121)      825 2022-06-20 07:52:36.000000 rithm-9.4.0/src/big_int/bit_length.rs
+-rw-r--r--   0 runner    (1001) docker     (121)     1934 2022-06-20 07:52:36.000000 rithm-9.4.0/src/big_int/bit_or.rs
+-rw-r--r--   0 runner    (1001) docker     (121)      899 2022-06-20 07:52:36.000000 rithm-9.4.0/src/big_int/bit_or_assign.rs
+-rw-r--r--   0 runner    (1001) docker     (121)     2040 2022-06-20 07:52:36.000000 rithm-9.4.0/src/big_int/bit_xor.rs
+-rw-r--r--   0 runner    (1001) docker     (121)      934 2022-06-20 07:52:36.000000 rithm-9.4.0/src/big_int/bit_xor_assign.rs
+-rw-r--r--   0 runner    (1001) docker     (121)     1782 2022-06-20 07:52:36.000000 rithm-9.4.0/src/big_int/checked_div.rs
+-rw-r--r--   0 runner    (1001) docker     (121)     1929 2022-06-20 07:52:36.000000 rithm-9.4.0/src/big_int/checked_div_as_f32.rs
+-rw-r--r--   0 runner    (1001) docker     (121)     1929 2022-06-20 07:52:36.000000 rithm-9.4.0/src/big_int/checked_div_as_f64.rs
+-rw-r--r--   0 runner    (1001) docker     (121)     1905 2022-06-20 07:52:36.000000 rithm-9.4.0/src/big_int/checked_div_euclid.rs
+-rw-r--r--   0 runner    (1001) docker     (121)     3551 2022-06-20 07:52:36.000000 rithm-9.4.0/src/big_int/checked_div_rem.rs
+-rw-r--r--   0 runner    (1001) docker     (121)     3946 2022-06-20 07:52:36.000000 rithm-9.4.0/src/big_int/checked_div_rem_euclid.rs
+-rw-r--r--   0 runner    (1001) docker     (121)     4556 2022-06-20 07:52:36.000000 rithm-9.4.0/src/big_int/checked_pow.rs
+-rw-r--r--   0 runner    (1001) docker     (121)    12701 2022-06-20 07:52:36.000000 rithm-9.4.0/src/big_int/checked_pow_rem_euclid.rs
+-rw-r--r--   0 runner    (1001) docker     (121)     1782 2022-06-20 07:52:36.000000 rithm-9.4.0/src/big_int/checked_rem.rs
+-rw-r--r--   0 runner    (1001) docker     (121)     1905 2022-06-20 07:52:36.000000 rithm-9.4.0/src/big_int/checked_rem_euclid.rs
+-rw-r--r--   0 runner    (1001) docker     (121)     2209 2022-06-20 07:52:36.000000 rithm-9.4.0/src/big_int/checked_rem_euclid_inv.rs
+-rw-r--r--   0 runner    (1001) docker     (121)     5736 2022-06-20 07:52:36.000000 rithm-9.4.0/src/big_int/checked_shl.rs
+-rw-r--r--   0 runner    (1001) docker     (121)     6324 2022-06-20 07:52:36.000000 rithm-9.4.0/src/big_int/checked_shr.rs
+-rw-r--r--   0 runner    (1001) docker     (121)      299 2022-06-20 07:52:36.000000 rithm-9.4.0/src/big_int/constants.rs
+-rw-r--r--   0 runner    (1001) docker     (121)      278 2022-06-20 07:52:36.000000 rithm-9.4.0/src/big_int/contracts.rs
+-rw-r--r--   0 runner    (1001) docker     (121)    74998 2022-06-20 07:52:36.000000 rithm-9.4.0/src/big_int/digits.rs
+-rw-r--r--   0 runner    (1001) docker     (121)     3129 2022-06-20 07:52:36.000000 rithm-9.4.0/src/big_int/display.rs
+-rw-r--r--   0 runner    (1001) docker     (121)     2222 2022-06-20 07:52:36.000000 rithm-9.4.0/src/big_int/div.rs
+-rw-r--r--   0 runner    (1001) docker     (121)      903 2022-06-20 07:52:36.000000 rithm-9.4.0/src/big_int/div_assign.rs
+-rw-r--r--   0 runner    (1001) docker     (121)     2252 2022-06-20 07:52:36.000000 rithm-9.4.0/src/big_int/div_euclid.rs
+-rw-r--r--   0 runner    (1001) docker     (121)     1618 2022-06-20 07:52:36.000000 rithm-9.4.0/src/big_int/div_rem.rs
+-rw-r--r--   0 runner    (1001) docker     (121)     1740 2022-06-20 07:52:36.000000 rithm-9.4.0/src/big_int/div_rem_euclid.rs
+-rw-r--r--   0 runner    (1001) docker     (121)      708 2022-06-20 07:52:36.000000 rithm-9.4.0/src/big_int/float_to_int.rs
+-rw-r--r--   0 runner    (1001) docker     (121)     1129 2022-06-20 07:52:36.000000 rithm-9.4.0/src/big_int/from.rs
+-rw-r--r--   0 runner    (1001) docker     (121)     1315 2022-06-20 07:52:36.000000 rithm-9.4.0/src/big_int/from_bytes.rs
+-rw-r--r--   0 runner    (1001) docker     (121)      711 2022-06-20 07:52:36.000000 rithm-9.4.0/src/big_int/from_str_radix.rs
+-rw-r--r--   0 runner    (1001) docker     (121)     1490 2022-06-20 07:52:36.000000 rithm-9.4.0/src/big_int/gcd.rs
+-rw-r--r--   0 runner    (1001) docker     (121)      286 2022-06-20 07:52:36.000000 rithm-9.4.0/src/big_int/hash.rs
+-rw-r--r--   0 runner    (1001) docker     (121)      478 2022-06-20 07:52:36.000000 rithm-9.4.0/src/big_int/is_power_of_two.rs
+-rw-r--r--   0 runner    (1001) docker     (121)     1071 2022-06-20 07:52:36.000000 rithm-9.4.0/src/big_int/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (121)     1673 2022-06-20 07:52:36.000000 rithm-9.4.0/src/big_int/mul.rs
+-rw-r--r--   0 runner    (1001) docker     (121)      715 2022-06-20 07:52:36.000000 rithm-9.4.0/src/big_int/mul_assign.rs
+-rw-r--r--   0 runner    (1001) docker     (121)      617 2022-06-20 07:52:36.000000 rithm-9.4.0/src/big_int/neg.rs
+-rw-r--r--   0 runner    (1001) docker     (121)      751 2022-06-20 07:52:36.000000 rithm-9.4.0/src/big_int/not.rs
+-rw-r--r--   0 runner    (1001) docker     (121)      448 2022-06-20 07:52:36.000000 rithm-9.4.0/src/big_int/ord.rs
+-rw-r--r--   0 runner    (1001) docker     (121)      391 2022-06-20 07:52:36.000000 rithm-9.4.0/src/big_int/parity.rs
+-rw-r--r--   0 runner    (1001) docker     (121)     1272 2022-06-20 07:52:36.000000 rithm-9.4.0/src/big_int/partial_eq.rs
+-rw-r--r--   0 runner    (1001) docker     (121)    14595 2022-06-20 07:52:36.000000 rithm-9.4.0/src/big_int/partial_ord.rs
+-rw-r--r--   0 runner    (1001) docker     (121)     1422 2022-06-20 07:52:36.000000 rithm-9.4.0/src/big_int/pow.rs
+-rw-r--r--   0 runner    (1001) docker     (121)     1997 2022-06-20 07:52:36.000000 rithm-9.4.0/src/big_int/rem.rs
+-rw-r--r--   0 runner    (1001) docker     (121)      903 2022-06-20 07:52:36.000000 rithm-9.4.0/src/big_int/rem_assign.rs
+-rw-r--r--   0 runner    (1001) docker     (121)     2252 2022-06-20 07:52:36.000000 rithm-9.4.0/src/big_int/rem_euclid.rs
+-rw-r--r--   0 runner    (1001) docker     (121)      332 2022-06-20 07:52:36.000000 rithm-9.4.0/src/big_int/signed.rs
+-rw-r--r--   0 runner    (1001) docker     (121)     1939 2022-06-20 07:52:36.000000 rithm-9.4.0/src/big_int/sub.rs
+-rw-r--r--   0 runner    (1001) docker     (121)      863 2022-06-20 07:52:36.000000 rithm-9.4.0/src/big_int/sub_assign.rs
+-rw-r--r--   0 runner    (1001) docker     (121)     1405 2022-06-20 07:52:36.000000 rithm-9.4.0/src/big_int/to_bytes.rs
+-rw-r--r--   0 runner    (1001) docker     (121)     1682 2022-06-20 07:52:36.000000 rithm-9.4.0/src/big_int/try_from.rs
+-rw-r--r--   0 runner    (1001) docker     (121)     5116 2022-06-20 07:52:36.000000 rithm-9.4.0/src/big_int/try_from_string.rs
+-rw-r--r--   0 runner    (1001) docker     (121)     4703 2022-06-20 07:52:36.000000 rithm-9.4.0/src/big_int/try_into.rs
+-rw-r--r--   0 runner    (1001) docker     (121)     7774 2022-06-20 07:52:36.000000 rithm-9.4.0/src/big_int/types.rs
+-rw-r--r--   0 runner    (1001) docker     (121)      428 2022-06-20 07:52:36.000000 rithm-9.4.0/src/big_int/unitary.rs
+-rw-r--r--   0 runner    (1001) docker     (121)      378 2022-06-20 07:52:36.000000 rithm-9.4.0/src/big_int/zeroable.rs
+-rw-r--r--   0 runner    (1001) docker     (121)       92 2022-06-20 07:52:36.000000 rithm-9.4.0/src/constants.rs
+-rw-r--r--   0 runner    (1001) docker     (121)      520 2022-06-20 07:52:36.000000 rithm-9.4.0/src/contracts.rs
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-20 07:52:58.120713 rithm-9.4.0/src/fraction/
+-rw-r--r--   0 runner    (1001) docker     (121)      350 2022-06-20 07:52:36.000000 rithm-9.4.0/src/fraction/abs.rs
+-rw-r--r--   0 runner    (1001) docker     (121)     1931 2022-06-20 07:52:36.000000 rithm-9.4.0/src/fraction/add.rs
+-rw-r--r--   0 runner    (1001) docker     (121)     1083 2022-06-20 07:52:36.000000 rithm-9.4.0/src/fraction/add_assign.rs
+-rw-r--r--   0 runner    (1001) docker     (121)      581 2022-06-20 07:52:36.000000 rithm-9.4.0/src/fraction/ceil.rs
+-rw-r--r--   0 runner    (1001) docker     (121)     3137 2022-06-20 07:52:36.000000 rithm-9.4.0/src/fraction/checked_div.rs
+-rw-r--r--   0 runner    (1001) docker     (121)     1765 2022-06-20 07:52:36.000000 rithm-9.4.0/src/fraction/checked_div_euclid.rs
+-rw-r--r--   0 runner    (1001) docker     (121)     3845 2022-06-20 07:52:36.000000 rithm-9.4.0/src/fraction/checked_div_rem_euclid.rs
+-rw-r--r--   0 runner    (1001) docker     (121)     1795 2022-06-20 07:52:36.000000 rithm-9.4.0/src/fraction/checked_pow.rs
+-rw-r--r--   0 runner    (1001) docker     (121)     3147 2022-06-20 07:52:36.000000 rithm-9.4.0/src/fraction/checked_rem.rs
+-rw-r--r--   0 runner    (1001) docker     (121)     3307 2022-06-20 07:52:36.000000 rithm-9.4.0/src/fraction/checked_rem_euclid.rs
+-rw-r--r--   0 runner    (1001) docker     (121)      701 2022-06-20 07:52:36.000000 rithm-9.4.0/src/fraction/debug.rs
+-rw-r--r--   0 runner    (1001) docker     (121)      438 2022-06-20 07:52:36.000000 rithm-9.4.0/src/fraction/display.rs
+-rw-r--r--   0 runner    (1001) docker     (121)     1661 2022-06-20 07:52:36.000000 rithm-9.4.0/src/fraction/div.rs
+-rw-r--r--   0 runner    (1001) docker     (121)     1247 2022-06-20 07:52:36.000000 rithm-9.4.0/src/fraction/div_assign.rs
+-rw-r--r--   0 runner    (1001) docker     (121)     1977 2022-06-20 07:52:36.000000 rithm-9.4.0/src/fraction/div_euclid.rs
+-rw-r--r--   0 runner    (1001) docker     (121)       87 2022-06-20 07:52:36.000000 rithm-9.4.0/src/fraction/eq.rs
+-rw-r--r--   0 runner    (1001) docker     (121)      478 2022-06-20 07:52:36.000000 rithm-9.4.0/src/fraction/floor.rs
+-rw-r--r--   0 runner    (1001) docker     (121)      279 2022-06-20 07:52:36.000000 rithm-9.4.0/src/fraction/from.rs
+-rw-r--r--   0 runner    (1001) docker     (121)      251 2022-06-20 07:52:36.000000 rithm-9.4.0/src/fraction/hash.rs
+-rw-r--r--   0 runner    (1001) docker     (121)      541 2022-06-20 07:52:36.000000 rithm-9.4.0/src/fraction/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (121)     1816 2022-06-20 07:52:36.000000 rithm-9.4.0/src/fraction/mul.rs
+-rw-r--r--   0 runner    (1001) docker     (121)     1115 2022-06-20 07:52:36.000000 rithm-9.4.0/src/fraction/mul_assign.rs
+-rw-r--r--   0 runner    (1001) docker     (121)      362 2022-06-20 07:52:36.000000 rithm-9.4.0/src/fraction/neg.rs
+-rw-r--r--   0 runner    (1001) docker     (121)      419 2022-06-20 07:52:36.000000 rithm-9.4.0/src/fraction/ord.rs
+-rw-r--r--   0 runner    (1001) docker     (121)     1224 2022-06-20 07:52:36.000000 rithm-9.4.0/src/fraction/partial_eq.rs
+-rw-r--r--   0 runner    (1001) docker     (121)     3995 2022-06-20 07:52:36.000000 rithm-9.4.0/src/fraction/partial_ord.rs
+-rw-r--r--   0 runner    (1001) docker     (121)      986 2022-06-20 07:52:36.000000 rithm-9.4.0/src/fraction/pow.rs
+-rw-r--r--   0 runner    (1001) docker     (121)     1885 2022-06-20 07:52:36.000000 rithm-9.4.0/src/fraction/rem.rs
+-rw-r--r--   0 runner    (1001) docker     (121)     1490 2022-06-20 07:52:36.000000 rithm-9.4.0/src/fraction/rem_assign.rs
+-rw-r--r--   0 runner    (1001) docker     (121)     1987 2022-06-20 07:52:36.000000 rithm-9.4.0/src/fraction/rem_euclid.rs
+-rw-r--r--   0 runner    (1001) docker     (121)     1492 2022-06-20 07:52:36.000000 rithm-9.4.0/src/fraction/round.rs
+-rw-r--r--   0 runner    (1001) docker     (121)      304 2022-06-20 07:52:36.000000 rithm-9.4.0/src/fraction/signed.rs
+-rw-r--r--   0 runner    (1001) docker     (121)     2595 2022-06-20 07:52:36.000000 rithm-9.4.0/src/fraction/sub.rs
+-rw-r--r--   0 runner    (1001) docker     (121)     1126 2022-06-20 07:52:36.000000 rithm-9.4.0/src/fraction/sub_assign.rs
+-rw-r--r--   0 runner    (1001) docker     (121)      451 2022-06-20 07:52:36.000000 rithm-9.4.0/src/fraction/trunc.rs
+-rw-r--r--   0 runner    (1001) docker     (121)     4719 2022-06-20 07:52:36.000000 rithm-9.4.0/src/fraction/try_from.rs
+-rw-r--r--   0 runner    (1001) docker     (121)      987 2022-06-20 07:52:36.000000 rithm-9.4.0/src/fraction/try_into.rs
+-rw-r--r--   0 runner    (1001) docker     (121)     2378 2022-06-20 07:52:36.000000 rithm-9.4.0/src/fraction/types.rs
+-rw-r--r--   0 runner    (1001) docker     (121)      364 2022-06-20 07:52:36.000000 rithm-9.4.0/src/fraction/unitary.rs
+-rw-r--r--   0 runner    (1001) docker     (121)      363 2022-06-20 07:52:36.000000 rithm-9.4.0/src/fraction/zero.rs
+-rw-r--r--   0 runner    (1001) docker     (121)    43036 2022-06-20 07:52:36.000000 rithm-9.4.0/src/lib.rs
+-rw-r--r--   0 runner    (1001) docker     (121)    39513 2022-06-20 07:52:36.000000 rithm-9.4.0/src/traits.rs
```

### Comparing `rithm-9.3.0/LICENSE` & `rithm-9.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rithm-9.3.0/PKG-INFO` & `rithm-9.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rithm
-Version: 9.3.0
+Version: 9.4.0
 Summary: Arbitrary precision arithmetic.
 Home-page: https://github.com/lycantropos/rithm/
 Download-URL: https://github.com/lycantropos/rithm/archive/master.zip
 Author: Azat Ibrakov
 Author-email: azatibrakov@gmail.com
 License: MIT License
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `rithm-9.3.0/README.md` & `rithm-9.4.0/README.md`

 * *Files identical despite different names*

### Comparing `rithm-9.3.0/rithm/__init__.pyi` & `rithm-9.4.0/rithm/__init__.pyi`

 * *Files identical despite different names*

### Comparing `rithm-9.3.0/rithm/_rithm.py` & `rithm-9.4.0/rithm/_rithm.py`

 * *Files identical despite different names*

### Comparing `rithm-9.3.0/rithm.egg-info/PKG-INFO` & `rithm-9.4.0/rithm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rithm
-Version: 9.3.0
+Version: 9.4.0
 Summary: Arbitrary precision arithmetic.
 Home-page: https://github.com/lycantropos/rithm/
 Download-URL: https://github.com/lycantropos/rithm/archive/master.zip
 Author: Azat Ibrakov
 Author-email: azatibrakov@gmail.com
 License: MIT License
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `rithm-9.3.0/rithm.egg-info/SOURCES.txt` & `rithm-9.4.0/rithm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rithm-9.3.0/setup.py` & `rithm-9.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `rithm-9.3.0/src/big_int/abs.rs` & `rithm-9.4.0/src/big_int/abs.rs`

 * *Files identical despite different names*

### Comparing `rithm-9.3.0/src/big_int/add.rs` & `rithm-9.4.0/src/big_int/add.rs`

 * *Files identical despite different names*

### Comparing `rithm-9.3.0/src/big_int/add_assign.rs` & `rithm-9.4.0/src/big_int/add_assign.rs`

 * *Files identical despite different names*

### Comparing `rithm-9.3.0/src/big_int/bit_and.rs` & `rithm-9.4.0/src/big_int/bit_and.rs`

 * *Files identical despite different names*

### Comparing `rithm-9.3.0/src/big_int/bit_and_assign.rs` & `rithm-9.4.0/src/big_int/bit_and_assign.rs`

 * *Files identical despite different names*

### Comparing `rithm-9.3.0/src/big_int/bit_length.rs` & `rithm-9.4.0/src/big_int/bit_length.rs`

 * *Files identical despite different names*

### Comparing `rithm-9.3.0/src/big_int/bit_or.rs` & `rithm-9.4.0/src/big_int/bit_or.rs`

 * *Files identical despite different names*

### Comparing `rithm-9.3.0/src/big_int/bit_or_assign.rs` & `rithm-9.4.0/src/big_int/bit_or_assign.rs`

 * *Files identical despite different names*

### Comparing `rithm-9.3.0/src/big_int/bit_xor.rs` & `rithm-9.4.0/src/big_int/bit_xor.rs`

 * *Files identical despite different names*

### Comparing `rithm-9.3.0/src/big_int/bit_xor_assign.rs` & `rithm-9.4.0/src/big_int/bit_xor_assign.rs`

 * *Files identical despite different names*

### Comparing `rithm-9.3.0/src/big_int/checked_div.rs` & `rithm-9.4.0/src/big_int/checked_div.rs`

 * *Files identical despite different names*

### Comparing `rithm-9.3.0/src/big_int/checked_div_as_f32.rs` & `rithm-9.4.0/src/big_int/checked_div_as_f32.rs`

 * *Files identical despite different names*

### Comparing `rithm-9.3.0/src/big_int/checked_div_as_f64.rs` & `rithm-9.4.0/src/big_int/checked_div_as_f64.rs`

 * *Files identical despite different names*

### Comparing `rithm-9.3.0/src/big_int/checked_div_euclid.rs` & `rithm-9.4.0/src/big_int/checked_div_euclid.rs`

 * *Files identical despite different names*

### Comparing `rithm-9.3.0/src/big_int/checked_div_rem.rs` & `rithm-9.4.0/src/big_int/checked_div_rem.rs`

 * *Files identical despite different names*

### Comparing `rithm-9.3.0/src/big_int/checked_div_rem_euclid.rs` & `rithm-9.4.0/src/big_int/checked_div_rem_euclid.rs`

 * *Files identical despite different names*

### Comparing `rithm-9.3.0/src/big_int/checked_pow.rs` & `rithm-9.4.0/src/big_int/checked_pow.rs`

 * *Files identical despite different names*

### Comparing `rithm-9.3.0/src/big_int/checked_pow_rem_euclid.rs` & `rithm-9.4.0/src/big_int/checked_pow_rem_euclid.rs`

 * *Files identical despite different names*

### Comparing `rithm-9.3.0/src/big_int/checked_rem.rs` & `rithm-9.4.0/src/big_int/checked_rem.rs`

 * *Files identical despite different names*

### Comparing `rithm-9.3.0/src/big_int/checked_rem_euclid.rs` & `rithm-9.4.0/src/big_int/checked_rem_euclid.rs`

 * *Files identical despite different names*

### Comparing `rithm-9.3.0/src/big_int/checked_rem_euclid_inv.rs` & `rithm-9.4.0/src/big_int/checked_rem_euclid_inv.rs`

 * *Files identical despite different names*

### Comparing `rithm-9.3.0/src/big_int/checked_shl.rs` & `rithm-9.4.0/src/big_int/checked_shl.rs`

 * *Files identical despite different names*

### Comparing `rithm-9.3.0/src/big_int/checked_shr.rs` & `rithm-9.4.0/src/big_int/checked_shr.rs`

 * *Files identical despite different names*

### Comparing `rithm-9.3.0/src/big_int/digits.rs` & `rithm-9.4.0/src/big_int/digits.rs`

 * *Files identical despite different names*

### Comparing `rithm-9.3.0/src/big_int/display.rs` & `rithm-9.4.0/src/big_int/display.rs`

 * *Files identical despite different names*

### Comparing `rithm-9.3.0/src/big_int/div.rs` & `rithm-9.4.0/src/big_int/div.rs`

 * *Files identical despite different names*

### Comparing `rithm-9.3.0/src/big_int/div_assign.rs` & `rithm-9.4.0/src/big_int/div_assign.rs`

 * *Files identical despite different names*

### Comparing `rithm-9.3.0/src/big_int/div_euclid.rs` & `rithm-9.4.0/src/big_int/div_euclid.rs`

 * *Files identical despite different names*

### Comparing `rithm-9.3.0/src/big_int/div_rem.rs` & `rithm-9.4.0/src/big_int/div_rem.rs`

 * *Files identical despite different names*

### Comparing `rithm-9.3.0/src/big_int/div_rem_euclid.rs` & `rithm-9.4.0/src/big_int/div_rem_euclid.rs`

 * *Files identical despite different names*

### Comparing `rithm-9.3.0/src/big_int/float_to_int.rs` & `rithm-9.4.0/src/big_int/float_to_int.rs`

 * *Files identical despite different names*

### Comparing `rithm-9.3.0/src/big_int/from_bytes.rs` & `rithm-9.4.0/src/big_int/from_bytes.rs`

 * *Files identical despite different names*

### Comparing `rithm-9.3.0/src/big_int/from_str_radix.rs` & `rithm-9.4.0/src/big_int/from_str_radix.rs`

 * *Files identical despite different names*

### Comparing `rithm-9.3.0/src/big_int/gcd.rs` & `rithm-9.4.0/src/big_int/gcd.rs`

 * *Files identical despite different names*

### Comparing `rithm-9.3.0/src/big_int/mod.rs` & `rithm-9.4.0/src/big_int/mod.rs`

 * *Files identical despite different names*

### Comparing `rithm-9.3.0/src/big_int/mul.rs` & `rithm-9.4.0/src/big_int/mul.rs`

 * *Files identical despite different names*

### Comparing `rithm-9.3.0/src/big_int/mul_assign.rs` & `rithm-9.4.0/src/big_int/mul_assign.rs`

 * *Files identical despite different names*

### Comparing `rithm-9.3.0/src/big_int/neg.rs` & `rithm-9.4.0/src/big_int/neg.rs`

 * *Files identical despite different names*

### Comparing `rithm-9.3.0/src/big_int/not.rs` & `rithm-9.4.0/src/big_int/not.rs`

 * *Files identical despite different names*

### Comparing `rithm-9.3.0/src/big_int/partial_eq.rs` & `rithm-9.4.0/src/big_int/partial_eq.rs`

 * *Files identical despite different names*

### Comparing `rithm-9.3.0/src/big_int/partial_ord.rs` & `rithm-9.4.0/src/big_int/partial_ord.rs`

 * *Files identical despite different names*

### Comparing `rithm-9.3.0/src/big_int/pow.rs` & `rithm-9.4.0/src/big_int/pow.rs`

 * *Files identical despite different names*

### Comparing `rithm-9.3.0/src/big_int/rem.rs` & `rithm-9.4.0/src/big_int/rem.rs`

 * *Files identical despite different names*

### Comparing `rithm-9.3.0/src/big_int/rem_assign.rs` & `rithm-9.4.0/src/big_int/rem_assign.rs`

 * *Files identical despite different names*

### Comparing `rithm-9.3.0/src/big_int/rem_euclid.rs` & `rithm-9.4.0/src/big_int/rem_euclid.rs`

 * *Files identical despite different names*

### Comparing `rithm-9.3.0/src/big_int/sub.rs` & `rithm-9.4.0/src/big_int/sub.rs`

 * *Files identical despite different names*

### Comparing `rithm-9.3.0/src/big_int/sub_assign.rs` & `rithm-9.4.0/src/big_int/sub_assign.rs`

 * *Files identical despite different names*

### Comparing `rithm-9.3.0/src/big_int/to_bytes.rs` & `rithm-9.4.0/src/big_int/to_bytes.rs`

 * *Files identical despite different names*

### Comparing `rithm-9.3.0/src/big_int/try_from.rs` & `rithm-9.4.0/src/big_int/try_from.rs`

 * *Files identical despite different names*

### Comparing `rithm-9.3.0/src/big_int/try_from_string.rs` & `rithm-9.4.0/src/big_int/try_from_string.rs`

 * *Files identical despite different names*

### Comparing `rithm-9.3.0/src/big_int/try_into.rs` & `rithm-9.4.0/src/big_int/try_into.rs`

 * *Files identical despite different names*

### Comparing `rithm-9.3.0/src/big_int/types.rs` & `rithm-9.4.0/src/big_int/types.rs`

 * *Files identical despite different names*

### Comparing `rithm-9.3.0/src/contracts.rs` & `rithm-9.4.0/src/contracts.rs`

 * *Files identical despite different names*

### Comparing `rithm-9.3.0/src/fraction/add.rs` & `rithm-9.4.0/src/fraction/add.rs`

 * *Files identical despite different names*

### Comparing `rithm-9.3.0/src/fraction/add_assign.rs` & `rithm-9.4.0/src/fraction/add_assign.rs`

 * *Files identical despite different names*

### Comparing `rithm-9.3.0/src/fraction/ceil.rs` & `rithm-9.4.0/src/fraction/ceil.rs`

 * *Files identical despite different names*

### Comparing `rithm-9.3.0/src/fraction/checked_div.rs` & `rithm-9.4.0/src/fraction/checked_div.rs`

 * *Files identical despite different names*

### Comparing `rithm-9.3.0/src/fraction/checked_div_euclid.rs` & `rithm-9.4.0/src/fraction/checked_div_euclid.rs`

 * *Files identical despite different names*

### Comparing `rithm-9.3.0/src/fraction/checked_div_rem_euclid.rs` & `rithm-9.4.0/src/fraction/checked_div_rem_euclid.rs`

 * *Files identical despite different names*

### Comparing `rithm-9.3.0/src/fraction/checked_pow.rs` & `rithm-9.4.0/src/fraction/checked_pow.rs`

 * *Files identical despite different names*

### Comparing `rithm-9.3.0/src/fraction/checked_rem.rs` & `rithm-9.4.0/src/fraction/checked_rem.rs`

 * *Files identical despite different names*

### Comparing `rithm-9.3.0/src/fraction/checked_rem_euclid.rs` & `rithm-9.4.0/src/fraction/checked_rem_euclid.rs`

 * *Files identical despite different names*

### Comparing `rithm-9.3.0/src/fraction/debug.rs` & `rithm-9.4.0/src/fraction/debug.rs`

 * *Files identical despite different names*

### Comparing `rithm-9.3.0/src/fraction/div.rs` & `rithm-9.4.0/src/fraction/div.rs`

 * *Files identical despite different names*

### Comparing `rithm-9.3.0/src/fraction/div_assign.rs` & `rithm-9.4.0/src/fraction/div_assign.rs`

 * *Files identical despite different names*

### Comparing `rithm-9.3.0/src/fraction/div_euclid.rs` & `rithm-9.4.0/src/fraction/div_euclid.rs`

 * *Files identical despite different names*

### Comparing `rithm-9.3.0/src/fraction/mod.rs` & `rithm-9.4.0/src/fraction/mod.rs`

 * *Files identical despite different names*

### Comparing `rithm-9.3.0/src/fraction/mul.rs` & `rithm-9.4.0/src/fraction/mul.rs`

 * *Files identical despite different names*

### Comparing `rithm-9.3.0/src/fraction/mul_assign.rs` & `rithm-9.4.0/src/fraction/mul_assign.rs`

 * *Files identical despite different names*

### Comparing `rithm-9.3.0/src/fraction/partial_eq.rs` & `rithm-9.4.0/src/fraction/partial_eq.rs`

 * *Files identical despite different names*

### Comparing `rithm-9.3.0/src/fraction/partial_ord.rs` & `rithm-9.4.0/src/fraction/partial_ord.rs`

 * *Files identical despite different names*

### Comparing `rithm-9.3.0/src/fraction/pow.rs` & `rithm-9.4.0/src/fraction/pow.rs`

 * *Files identical despite different names*

### Comparing `rithm-9.3.0/src/fraction/rem.rs` & `rithm-9.4.0/src/fraction/rem.rs`

 * *Files identical despite different names*

### Comparing `rithm-9.3.0/src/fraction/rem_assign.rs` & `rithm-9.4.0/src/fraction/rem_assign.rs`

 * *Files identical despite different names*

### Comparing `rithm-9.3.0/src/fraction/rem_euclid.rs` & `rithm-9.4.0/src/fraction/rem_euclid.rs`

 * *Files identical despite different names*

### Comparing `rithm-9.3.0/src/fraction/round.rs` & `rithm-9.4.0/src/fraction/round.rs`

 * *Files identical despite different names*

### Comparing `rithm-9.3.0/src/fraction/sub.rs` & `rithm-9.4.0/src/fraction/sub.rs`

 * *Files identical despite different names*

### Comparing `rithm-9.3.0/src/fraction/sub_assign.rs` & `rithm-9.4.0/src/fraction/sub_assign.rs`

 * *Files identical despite different names*

### Comparing `rithm-9.3.0/src/fraction/try_from.rs` & `rithm-9.4.0/src/fraction/try_from.rs`

 * *Files identical despite different names*

### Comparing `rithm-9.3.0/src/fraction/try_into.rs` & `rithm-9.4.0/src/fraction/try_into.rs`

 * *Files identical despite different names*

### Comparing `rithm-9.3.0/src/fraction/types.rs` & `rithm-9.4.0/src/fraction/types.rs`

 * *Files identical despite different names*

### Comparing `rithm-9.3.0/src/lib.rs` & `rithm-9.4.0/src/lib.rs`

 * *Files identical despite different names*

### Comparing `rithm-9.3.0/src/traits.rs` & `rithm-9.4.0/src/traits.rs`

 * *Files identical despite different names*

