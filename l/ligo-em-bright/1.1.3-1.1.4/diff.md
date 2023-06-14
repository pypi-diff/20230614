# Comparing `tmp/ligo_em_bright-1.1.3.tar.gz` & `tmp/ligo_em_bright-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ligo_em_bright-1.1.3.tar", max compression
+gzip compressed data, was "ligo_em_bright-1.1.4.tar", max compression
```

## Comparing `ligo_em_bright-1.1.3.tar` & `ligo_em_bright-1.1.4.tar`

### file list

```diff
@@ -1,14 +1,18 @@
--rw-r--r--   0        0        0     1093 2023-03-15 17:51:21.569855 ligo_em_bright-1.1.3/LICENSE
--rw-r--r--   0        0        0      985 2023-03-15 17:51:21.569855 ligo_em_bright-1.1.3/README.md
--rw-r--r--   0        0        0      865 2023-05-24 19:32:44.968092 ligo_em_bright-1.1.3/ligo/em_bright/__init__.py
--rw-r--r--   0        0        0     9890 2023-04-07 01:33:56.185447 ligo_em_bright-1.1.3/ligo/em_bright/categorize.py
--rw-r--r--   0        0        0    10141 2023-04-07 01:33:56.185447 ligo_em_bright-1.1.3/ligo/em_bright/computeDiskMass.py
--rw-r--r--   0        0        0    15224 2023-04-07 01:33:56.185447 ligo_em_bright-1.1.3/ligo/em_bright/dag_writer.py
--rw-r--r--   0        0        0     2407 2023-04-07 01:33:56.185447 ligo_em_bright-1.1.3/ligo/em_bright/data/__init__.py
--rw-r--r--   0        0        0     8588 2023-05-24 19:22:27.251422 ligo_em_bright-1.1.3/ligo/em_bright/em_bright.py
--rw-r--r--   0        0        0        0 2023-03-15 17:51:21.925857 ligo_em_bright-1.1.3/ligo/em_bright/tests/__init__.py
--rw-r--r--   0        0        0      307 2023-03-15 17:51:21.925857 ligo_em_bright-1.1.3/ligo/em_bright/tests/data/test_categorize_data.tbl
--rw-r--r--   0        0        0     8756 2023-05-24 19:32:44.968092 ligo_em_bright-1.1.3/ligo/em_bright/tests/test_em_bright.py
--rw-r--r--   0        0        0    23921 2023-04-07 01:46:47.038281 ligo_em_bright-1.1.3/ligo/em_bright/utils.py
--rw-r--r--   0        0        0     1382 2023-05-24 19:32:44.968092 ligo_em_bright-1.1.3/pyproject.toml
--rw-r--r--   0        0        0     1700 1970-01-01 00:00:00.000000 ligo_em_bright-1.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-06-02 19:51:52.112296 ligo_em_bright-1.1.4/LICENSE
+-rw-r--r--   0        0        0      977 2023-06-02 19:51:52.113296 ligo_em_bright-1.1.4/README.md
+-rw-r--r--   0        0        0   301056 2023-06-02 20:46:02.409853 ligo_em_bright-1.1.4/ligo/em_bright/Bilby.posterior_samples.hdf5
+-rw-r--r--   0        0        0   354496 2023-06-13 15:16:31.735169 ligo_em_bright-1.1.4/ligo/em_bright/S230518h/Bilby.posterior_samples.hdf5
+-rw-r--r--   0        0        0   301056 2023-06-14 14:11:00.054801 ligo_em_bright-1.1.4/ligo/em_bright/S230529ay/Bilby.posterior_samples.hdf5
+-rw-r--r--   0        0        0      817 2023-06-14 19:07:57.536395 ligo_em_bright-1.1.4/ligo/em_bright/__init__.py
+-rw-r--r--   0        0        0     9617 2023-06-02 19:51:52.118296 ligo_em_bright-1.1.4/ligo/em_bright/categorize.py
+-rw-r--r--   0        0        0     9860 2023-06-13 22:09:14.360169 ligo_em_bright-1.1.4/ligo/em_bright/computeDiskMass.py
+-rw-r--r--   0        0        0    14843 2023-06-02 19:51:52.119296 ligo_em_bright-1.1.4/ligo/em_bright/dag_writer.py
+-rw-r--r--   0        0        0     2322 2023-06-02 19:51:53.643297 ligo_em_bright-1.1.4/ligo/em_bright/data/__init__.py
+-rw-r--r--   0        0        0     8609 2023-06-14 18:26:41.570242 ligo_em_bright-1.1.4/ligo/em_bright/em_bright.py
+-rw-r--r--   0        0        0        0 2023-06-02 19:51:53.645297 ligo_em_bright-1.1.4/ligo/em_bright/tests/__init__.py
+-rw-r--r--   0        0        0      303 2023-06-02 19:51:53.646297 ligo_em_bright-1.1.4/ligo/em_bright/tests/data/test_categorize_data.tbl
+-rw-r--r--   0        0        0    10368 2023-06-14 19:13:14.723545 ligo_em_bright-1.1.4/ligo/em_bright/tests/test_em_bright.py
+-rw-r--r--   0        0        0     1590 2023-06-02 20:46:13.007862 ligo_em_bright-1.1.4/ligo/em_bright/tests/test_sc_pe.py
+-rw-r--r--   0        0        0    23258 2023-06-02 19:51:53.648297 ligo_em_bright-1.1.4/ligo/em_bright/utils.py
+-rw-r--r--   0        0        0     1328 2023-06-14 19:07:32.375376 ligo_em_bright-1.1.4/pyproject.toml
+-rw-r--r--   0        0        0     1700 1970-01-01 00:00:00.000000 ligo_em_bright-1.1.4/PKG-INFO
```

### Comparing `ligo_em_bright-1.1.3/README.md` & `ligo_em_bright-1.1.4/README.md`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# ligo.em_bright
-
-This library provides the tools to compute the possibility of merging gravitational-wave binaries to have an electromagnetic counterpart or having a component in the lower mass-gap region. The data products are source properties
-- `HasNS`: The mass of at least one of the compact binary coalescence is consistent with a neutron star.
-- `HasRemnant`: A non-zero amount of remnant matter remained outside the final compact object (a necessary but not sufficient condition to produce certain kinds of electromagnetic emission such as a short GRB or a kilonova).
-- `HasMassGap`: The mass of at least one of the compact binary coalescence is consistent with lower mass-gap region i.e. between 3-5 solar mass.
-
-The `HasNS` and `HasRemnant` quantities depend on, and are marginalized over, several neutron star equations of state (EOS). The marginalization is done using data from [GW170817](https://www.gw-openscience.org/eventapi/html/GWTC-1-confident/GW170817/).
+# ligo.em_bright
+
+This library provides the tools to compute the possibility of merging gravitational-wave binaries to have an electromagnetic counterpart or having a component in the lower mass-gap region. The data products are source properties
+- `HasNS`: The mass of at least one of the compact binary coalescence is consistent with a neutron star.
+- `HasRemnant`: A non-zero amount of remnant matter remained outside the final compact object (a necessary but not sufficient condition to produce certain kinds of electromagnetic emission such as a short GRB or a kilonova).
+- `HasMassGap`: The mass of at least one of the compact binary coalescence is consistent with lower mass-gap region i.e. between 3-5 solar mass.
+
+The `HasNS` and `HasRemnant` quantities depend on, and are marginalized over, several neutron star equations of state (EOS). The marginalization is done using data from [GW170817](https://www.gw-openscience.org/eventapi/html/GWTC-1-confident/GW170817/).
```

### Comparing `ligo_em_bright-1.1.3/ligo/em_bright/categorize.py` & `ligo_em_bright-1.1.4/ligo/em_bright/categorize.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,273 +1,273 @@
-# Copyright (C) 2020 Shaon Ghosh, Deep Chatterjee
-#
-# This program is free software; you can redistribute it and/or modify it
-# under the terms of the GNU General Public License as published by the
-# Free Software Foundation; either version 2 of the License, or (at your
-# option) any later version.
-#
-# This program is distributed in the hope that it will be useful, but
-# WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU General
-# Public License for more details.
-#
-# You should have received a copy of the GNU General Public License along
-# with this program; if not, write to the Free Software Foundation, Inc.,
-# 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA.
-
-
-import argparse
-import functools
-import os
-
-import numpy as np
-import pandas as pd
-import pickle
-
-from . import computeDiskMass
-from .data import EOS_BAYES_FACTORS, EOS_MAX_MASS
-
-
-class _TupleHandler(object):
-    def __call__(self, func):
-        @functools.wraps(func)
-        def handle(*args, **kwargs):
-            try:
-                (infile, outfile, max_mass, eosname), *_ = args
-            except (ValueError, TypeError):
-                return func(*args, **kwargs)
-            return func(infile, outfile, max_mass, eosname)
-        return handle
-
-
-def regularize(m1, m2, chi1, chi2):
-    '''Transform masses based on the convention m1 > m2.
-    Apply the same for spins.
-    '''
-    # Find cases where the mass2 is greater than the mass1
-    largerMass1 = m1 >= m2
-    largerMass2 = m2 > m1
-
-    # Set up vectors to store the regularized masses and spins
-    m_primary = np.zeros_like(m1)
-    m_secondary = np.zeros_like(m2)
-    chi_primary = np.zeros_like(chi1)
-    chi_secondary = np.zeros_like(chi2)
-
-    # Swap vales of masses if mass1 < mass2
-    m_primary[largerMass1] = m1[largerMass1]
-    m_primary[~largerMass1] = m2[largerMass2]
-    m_secondary[~largerMass2] = m2[~largerMass2]
-    m_secondary[largerMass2] = m1[~largerMass1]
-
-    # Assign the spin values accordingly
-    chi_primary[largerMass1] = chi1[largerMass1]
-    chi_primary[~largerMass1] = chi2[~largerMass1]
-    chi_secondary[~largerMass2] = chi2[~largerMass2]
-    chi_secondary[largerMass2] = chi1[~largerMass1]
-
-    return (m_primary, m_secondary, chi_primary, chi_secondary)
-
-
-@_TupleHandler()
-def embright_categorization(inFile, outFile, eosname='2H', mNs_mass=None):
-    '''Categorize whether the binary has a neutron star, and any non-zero
-    remnant post merger, based on the ``eosname``.
-
-    Parameters
-    ----------
-    inFile : str
-        input filename
-    outFile : str
-        output filename
-    eosname : str
-        neutron star equation of state. Assumed implemented in lalsimulation.
-        Default 2H.
-    mNS_mass : float
-        Provide to override the maximum mass from ``eosname``.
-    '''
-    df = pd.read_table(inFile, delimiter='\t')
-    m1_inj, m1_rec = df.inj_m1.values, df.rec_m1.values
-    m2_inj, m2_rec = df.inj_m2.values, df.rec_m2.values
-    redshift_inj = df.inj_redshift.values
-    m1_inj_source = m1_inj / (1 + redshift_inj)
-    m2_inj_source = m2_inj / (1 + redshift_inj)
-
-    chi1_inj, chi1_rec = df.inj_spin1z.values, df.rec_spin1z.values
-    chi2_inj, chi2_rec = df.inj_spin2z.values, df.rec_spin2z.values
-    m1_inj, m2_inj, chi1_inj, chi2_inj = regularize(
-        m1_inj, m2_inj, chi1_inj, chi2_inj
-    )
-    m1_rec, m2_rec, chi1_rec, chi2_rec = regularize(
-        m1_rec, m2_rec, chi1_rec, chi2_rec
-    )
-    m1_inj_source, m2_inj_source, _, _ = regularize(
-        m1_inj_source, m2_inj_source, chi1_inj, chi2_inj
-    )  # spins regularized from previous step.
-    if mNs_mass:
-        NS_classified = m2_inj_source < mNs_mass
-    else:
-        NS_classified = m2_inj_source < EOS_MAX_MASS[eosname]
-    NS_classified = NS_classified.astype(int)
-
-    R_isco_hat_inj = computeDiskMass.compute_isco(chi1_inj)
-    R_isco_hat_rec = computeDiskMass.compute_isco(chi1_rec)
-
-    Compactness_inj, *_ = computeDiskMass.computeCompactness(m2_inj,
-                                                             eosname=eosname)
-    Compactness_rec, *_ = computeDiskMass.computeCompactness(m2_rec,
-                                                             eosname=eosname)
-
-    mc_inj = (m1_inj*m2_inj)**(3/5)/((m1_inj + m2_inj)**(1/5))
-    mc_rec = (m1_rec*m2_rec)**(3/5)/((m1_rec + m2_rec)**(1/5))
-
-    frac_mc_err = np.abs(mc_inj - mc_rec)/mc_inj
-
-    q_inj = m1_inj/m2_inj
-    q_rec = m1_rec/m2_rec
-
-    disk_mass_inj = computeDiskMass.computeDiskMass(
-        m1_inj_source, m2_inj_source, chi1_inj,
-        chi2_inj, eosname=eosname
-    )
-    EMB_classified = disk_mass_inj > 1e-3
-    EMB_classified = EMB_classified.astype(int)
-
-    output = np.vstack(
-        (m1_inj, m2_inj, chi1_inj, chi2_inj, redshift_inj,
-         mc_inj, q_inj, R_isco_hat_inj, Compactness_inj,
-         m1_rec, m2_rec, chi1_rec, chi2_rec,
-         mc_rec, frac_mc_err, q_rec, R_isco_hat_rec, Compactness_rec,
-         df.cfar.values, df.snr.values, df.gpstime.values, NS_classified,
-         EMB_classified)
-    ).T
-
-    df_complete = pd.DataFrame(output, columns=[
-        'm1_inj', 'm2_inj', 'chi1_inj', 'chi2_inj', 'inj_redshift',
-        'mc_inj', 'q_inj', 'R_isco_inj', 'Compactness_inj',
-        'm1_rec', 'm2_rec', 'chi1_rec', 'chi2_rec', 'mc_rec',
-        'frac_mc_err', 'q_rec', 'R_isco_rec', 'Compactness_rec',
-        'cfar', 'snr', 'gpstime', 'NS', 'EMB']
-    )
-    # drop NSs above max-mass
-    try:
-        max_mass = EOS_MAX_MASS[eosname]
-    except KeyError:
-        raise NotImplementedError
-    drop_mask = (m1_inj_source > max_mass) & (m1_inj_source < 3.0)  # noqa: E501; Restricts m2 by construction
-    df_complete = df_complete.loc[~drop_mask]
-    with open(outFile, 'wb') as f:
-        pickle.dump(df_complete, f)
-    return df_complete
-
-
-@_TupleHandler()
-def mass_gap_categorization(inFile, outFile):
-    '''Categorize whether the binary is in the lower mass gap
-    i.e., any component is between 3 and 5 solar mass
-
-    Parameters
-    ----------
-    inFile : str
-        input filename
-    outFile : str
-        output filename
-    '''
-    df = pd.read_table(inFile, delimiter='\t')
-    m1_inj, m1_rec = df.inj_m1.values, df.rec_m1.values
-    m2_inj, m2_rec = df.inj_m2.values, df.rec_m2.values
-    redshift_inj = df.inj_redshift.values
-    m1_inj_source = m1_inj / (1 + redshift_inj)
-    m2_inj_source = m2_inj / (1 + redshift_inj)
-
-    chi1_inj, chi1_rec = df.inj_spin1z.values, df.rec_spin1z.values
-    chi2_inj, chi2_rec = df.inj_spin2z.values, df.rec_spin2z.values
-    m1_inj, m2_inj, chi1_inj, chi2_inj = regularize(
-        m1_inj, m2_inj, chi1_inj, chi2_inj
-    )
-    m1_rec, m2_rec, chi1_rec, chi2_rec = regularize(
-        m1_rec, m2_rec, chi1_rec, chi2_rec
-    )
-    m1_inj_source, m2_inj_source, _, _ = regularize(
-        m1_inj_source, m2_inj_source, chi1_inj, chi2_inj
-    )  # spins regularized from previous step.
-    massgap_classified = (m1_inj_source > 3.0) & (m1_inj_source < 5.0)
-    massgap_classified += (m2_inj_source > 3.0) & (m2_inj_source < 5.0)
-    output = np.vstack(
-        (m1_inj_source, m2_inj_source, m1_inj, m2_inj, chi1_inj,
-         chi2_inj, redshift_inj, m1_rec, m2_rec, chi1_rec, chi2_rec,
-         df.cfar.values, df.snr.values, df.gpstime.values,
-         massgap_classified)
-    ).T
-
-    df_complete = pd.DataFrame(output, columns=[
-        'm1_inj_source', 'm2_inj_source', 'm1_inj', 'm2_inj', 'chi1_inj',
-        'chi2_inj', 'inj_redshift', 'm1_rec', 'm2_rec', 'chi1_rec',
-        'chi2_rec', 'cfar', 'snr', 'gpstime', 'mass_gap']
-    )
-    with open(outFile, 'wb') as f:
-        pickle.dump(df_complete, f)
-    return df_complete
-
-
-def main():
-    parser = argparse.ArgumentParser()
-    parser.add_argument("-i", "--input", action="store", type=str,
-                        help="Name of the input file")
-    parser.add_argument("-o", "--output", action="store", type=str,
-                        help="Name of the output file")
-    group = parser.add_mutually_exclusive_group()
-    group.add_argument(
-        "-e", "--eosname", default='2H',
-        help="Equation of state used compute remnant matter."
-    )
-    group.add_argument(
-        "--mass-gap", required=False, action="store_true",
-        default=False, help="Supply for mass gap categorization")
-
-    args = parser.parse_args()
-
-    if args.mass_gap:
-        mass_gap_categorization(args.input, args.output)
-    else:
-        embright_categorization(args.input, args.output,
-                                eosname=args.eosname)
-
-
-def main_all():
-    parser = argparse.ArgumentParser(
-        "Run categorization on all available EoSs: "
-        f"{EOS_BAYES_FACTORS.keys()}\n"
-        "Output will be tagged by EoS names."
-    )
-    parser.add_argument(
-        "-i", "--input", action="store", type=str,
-        help="Name of the input file"
-    )
-    parser.add_argument(
-        "-d", "--output-directory", type=str,
-        help="Output directory"
-    )
-    parser.add_argument(
-        "-o", "--output-prefix", action="store",
-        type=str, help="Input prefix "
-    )
-    parser.add_argument(
-        "-p", "--pool", default=1, type=int,
-        help="Pool size"
-    )
-    args = parser.parse_args()
-
-    from multiprocessing import Pool
-    eos_args = [
-        (
-            args.input, os.path.join(
-                args.output_directory,
-                f"{args.output_prefix}_{eosname}.pkl"
-            ),
-            EOS_MAX_MASS[eosname],
-            eosname
-        )
-        for eosname in EOS_BAYES_FACTORS
-    ]
-    with Pool(args.pool) as p:
-        p.map(embright_categorization, eos_args)
+# Copyright (C) 2020 Shaon Ghosh, Deep Chatterjee
+#
+# This program is free software; you can redistribute it and/or modify it
+# under the terms of the GNU General Public License as published by the
+# Free Software Foundation; either version 2 of the License, or (at your
+# option) any later version.
+#
+# This program is distributed in the hope that it will be useful, but
+# WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU General
+# Public License for more details.
+#
+# You should have received a copy of the GNU General Public License along
+# with this program; if not, write to the Free Software Foundation, Inc.,
+# 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA.
+
+
+import argparse
+import functools
+import os
+
+import numpy as np
+import pandas as pd
+import pickle
+
+from . import computeDiskMass
+from .data import EOS_BAYES_FACTORS, EOS_MAX_MASS
+
+
+class _TupleHandler(object):
+    def __call__(self, func):
+        @functools.wraps(func)
+        def handle(*args, **kwargs):
+            try:
+                (infile, outfile, max_mass, eosname), *_ = args
+            except (ValueError, TypeError):
+                return func(*args, **kwargs)
+            return func(infile, outfile, max_mass, eosname)
+        return handle
+
+
+def regularize(m1, m2, chi1, chi2):
+    '''Transform masses based on the convention m1 > m2.
+    Apply the same for spins.
+    '''
+    # Find cases where the mass2 is greater than the mass1
+    largerMass1 = m1 >= m2
+    largerMass2 = m2 > m1
+
+    # Set up vectors to store the regularized masses and spins
+    m_primary = np.zeros_like(m1)
+    m_secondary = np.zeros_like(m2)
+    chi_primary = np.zeros_like(chi1)
+    chi_secondary = np.zeros_like(chi2)
+
+    # Swap vales of masses if mass1 < mass2
+    m_primary[largerMass1] = m1[largerMass1]
+    m_primary[~largerMass1] = m2[largerMass2]
+    m_secondary[~largerMass2] = m2[~largerMass2]
+    m_secondary[largerMass2] = m1[~largerMass1]
+
+    # Assign the spin values accordingly
+    chi_primary[largerMass1] = chi1[largerMass1]
+    chi_primary[~largerMass1] = chi2[~largerMass1]
+    chi_secondary[~largerMass2] = chi2[~largerMass2]
+    chi_secondary[largerMass2] = chi1[~largerMass1]
+
+    return (m_primary, m_secondary, chi_primary, chi_secondary)
+
+
+@_TupleHandler()
+def embright_categorization(inFile, outFile, eosname='2H', mNs_mass=None):
+    '''Categorize whether the binary has a neutron star, and any non-zero
+    remnant post merger, based on the ``eosname``.
+
+    Parameters
+    ----------
+    inFile : str
+        input filename
+    outFile : str
+        output filename
+    eosname : str
+        neutron star equation of state. Assumed implemented in lalsimulation.
+        Default 2H.
+    mNS_mass : float
+        Provide to override the maximum mass from ``eosname``.
+    '''
+    df = pd.read_table(inFile, delimiter='\t')
+    m1_inj, m1_rec = df.inj_m1.values, df.rec_m1.values
+    m2_inj, m2_rec = df.inj_m2.values, df.rec_m2.values
+    redshift_inj = df.inj_redshift.values
+    m1_inj_source = m1_inj / (1 + redshift_inj)
+    m2_inj_source = m2_inj / (1 + redshift_inj)
+
+    chi1_inj, chi1_rec = df.inj_spin1z.values, df.rec_spin1z.values
+    chi2_inj, chi2_rec = df.inj_spin2z.values, df.rec_spin2z.values
+    m1_inj, m2_inj, chi1_inj, chi2_inj = regularize(
+        m1_inj, m2_inj, chi1_inj, chi2_inj
+    )
+    m1_rec, m2_rec, chi1_rec, chi2_rec = regularize(
+        m1_rec, m2_rec, chi1_rec, chi2_rec
+    )
+    m1_inj_source, m2_inj_source, _, _ = regularize(
+        m1_inj_source, m2_inj_source, chi1_inj, chi2_inj
+    )  # spins regularized from previous step.
+    if mNs_mass:
+        NS_classified = m2_inj_source < mNs_mass
+    else:
+        NS_classified = m2_inj_source < EOS_MAX_MASS[eosname]
+    NS_classified = NS_classified.astype(int)
+
+    R_isco_hat_inj = computeDiskMass.compute_isco(chi1_inj)
+    R_isco_hat_rec = computeDiskMass.compute_isco(chi1_rec)
+
+    Compactness_inj, *_ = computeDiskMass.computeCompactness(m2_inj,
+                                                             eosname=eosname)
+    Compactness_rec, *_ = computeDiskMass.computeCompactness(m2_rec,
+                                                             eosname=eosname)
+
+    mc_inj = (m1_inj*m2_inj)**(3/5)/((m1_inj + m2_inj)**(1/5))
+    mc_rec = (m1_rec*m2_rec)**(3/5)/((m1_rec + m2_rec)**(1/5))
+
+    frac_mc_err = np.abs(mc_inj - mc_rec)/mc_inj
+
+    q_inj = m1_inj/m2_inj
+    q_rec = m1_rec/m2_rec
+
+    disk_mass_inj = computeDiskMass.computeDiskMass(
+        m1_inj_source, m2_inj_source, chi1_inj,
+        chi2_inj, eosname=eosname
+    )
+    EMB_classified = disk_mass_inj > 1e-3
+    EMB_classified = EMB_classified.astype(int)
+
+    output = np.vstack(
+        (m1_inj, m2_inj, chi1_inj, chi2_inj, redshift_inj,
+         mc_inj, q_inj, R_isco_hat_inj, Compactness_inj,
+         m1_rec, m2_rec, chi1_rec, chi2_rec,
+         mc_rec, frac_mc_err, q_rec, R_isco_hat_rec, Compactness_rec,
+         df.cfar.values, df.snr.values, df.gpstime.values, NS_classified,
+         EMB_classified)
+    ).T
+
+    df_complete = pd.DataFrame(output, columns=[
+        'm1_inj', 'm2_inj', 'chi1_inj', 'chi2_inj', 'inj_redshift',
+        'mc_inj', 'q_inj', 'R_isco_inj', 'Compactness_inj',
+        'm1_rec', 'm2_rec', 'chi1_rec', 'chi2_rec', 'mc_rec',
+        'frac_mc_err', 'q_rec', 'R_isco_rec', 'Compactness_rec',
+        'cfar', 'snr', 'gpstime', 'NS', 'EMB']
+    )
+    # drop NSs above max-mass
+    try:
+        max_mass = EOS_MAX_MASS[eosname]
+    except KeyError:
+        raise NotImplementedError
+    drop_mask = (m1_inj_source > max_mass) & (m1_inj_source < 3.0)  # noqa: E501; Restricts m2 by construction
+    df_complete = df_complete.loc[~drop_mask]
+    with open(outFile, 'wb') as f:
+        pickle.dump(df_complete, f)
+    return df_complete
+
+
+@_TupleHandler()
+def mass_gap_categorization(inFile, outFile):
+    '''Categorize whether the binary is in the lower mass gap
+    i.e., any component is between 3 and 5 solar mass
+
+    Parameters
+    ----------
+    inFile : str
+        input filename
+    outFile : str
+        output filename
+    '''
+    df = pd.read_table(inFile, delimiter='\t')
+    m1_inj, m1_rec = df.inj_m1.values, df.rec_m1.values
+    m2_inj, m2_rec = df.inj_m2.values, df.rec_m2.values
+    redshift_inj = df.inj_redshift.values
+    m1_inj_source = m1_inj / (1 + redshift_inj)
+    m2_inj_source = m2_inj / (1 + redshift_inj)
+
+    chi1_inj, chi1_rec = df.inj_spin1z.values, df.rec_spin1z.values
+    chi2_inj, chi2_rec = df.inj_spin2z.values, df.rec_spin2z.values
+    m1_inj, m2_inj, chi1_inj, chi2_inj = regularize(
+        m1_inj, m2_inj, chi1_inj, chi2_inj
+    )
+    m1_rec, m2_rec, chi1_rec, chi2_rec = regularize(
+        m1_rec, m2_rec, chi1_rec, chi2_rec
+    )
+    m1_inj_source, m2_inj_source, _, _ = regularize(
+        m1_inj_source, m2_inj_source, chi1_inj, chi2_inj
+    )  # spins regularized from previous step.
+    massgap_classified = (m1_inj_source > 3.0) & (m1_inj_source < 5.0)
+    massgap_classified += (m2_inj_source > 3.0) & (m2_inj_source < 5.0)
+    output = np.vstack(
+        (m1_inj_source, m2_inj_source, m1_inj, m2_inj, chi1_inj,
+         chi2_inj, redshift_inj, m1_rec, m2_rec, chi1_rec, chi2_rec,
+         df.cfar.values, df.snr.values, df.gpstime.values,
+         massgap_classified)
+    ).T
+
+    df_complete = pd.DataFrame(output, columns=[
+        'm1_inj_source', 'm2_inj_source', 'm1_inj', 'm2_inj', 'chi1_inj',
+        'chi2_inj', 'inj_redshift', 'm1_rec', 'm2_rec', 'chi1_rec',
+        'chi2_rec', 'cfar', 'snr', 'gpstime', 'mass_gap']
+    )
+    with open(outFile, 'wb') as f:
+        pickle.dump(df_complete, f)
+    return df_complete
+
+
+def main():
+    parser = argparse.ArgumentParser()
+    parser.add_argument("-i", "--input", action="store", type=str,
+                        help="Name of the input file")
+    parser.add_argument("-o", "--output", action="store", type=str,
+                        help="Name of the output file")
+    group = parser.add_mutually_exclusive_group()
+    group.add_argument(
+        "-e", "--eosname", default='2H',
+        help="Equation of state used compute remnant matter."
+    )
+    group.add_argument(
+        "--mass-gap", required=False, action="store_true",
+        default=False, help="Supply for mass gap categorization")
+
+    args = parser.parse_args()
+
+    if args.mass_gap:
+        mass_gap_categorization(args.input, args.output)
+    else:
+        embright_categorization(args.input, args.output,
+                                eosname=args.eosname)
+
+
+def main_all():
+    parser = argparse.ArgumentParser(
+        "Run categorization on all available EoSs: "
+        f"{EOS_BAYES_FACTORS.keys()}\n"
+        "Output will be tagged by EoS names."
+    )
+    parser.add_argument(
+        "-i", "--input", action="store", type=str,
+        help="Name of the input file"
+    )
+    parser.add_argument(
+        "-d", "--output-directory", type=str,
+        help="Output directory"
+    )
+    parser.add_argument(
+        "-o", "--output-prefix", action="store",
+        type=str, help="Input prefix "
+    )
+    parser.add_argument(
+        "-p", "--pool", default=1, type=int,
+        help="Pool size"
+    )
+    args = parser.parse_args()
+
+    from multiprocessing import Pool
+    eos_args = [
+        (
+            args.input, os.path.join(
+                args.output_directory,
+                f"{args.output_prefix}_{eosname}.pkl"
+            ),
+            EOS_MAX_MASS[eosname],
+            eosname
+        )
+        for eosname in EOS_BAYES_FACTORS
+    ]
+    with Pool(args.pool) as p:
+        p.map(embright_categorization, eos_args)
```

### Comparing `ligo_em_bright-1.1.3/ligo/em_bright/computeDiskMass.py` & `ligo_em_bright-1.1.4/ligo/em_bright/computeDiskMass.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,291 +1,291 @@
-import numpy as np
-import astropy.units as u
-import astropy.constants as c
-from scipy.optimize import fsolve
-from scipy.interpolate import UnivariateSpline, interp1d
-
-import lal
-import lalsimulation as lalsim
-
-from .data import PACKAGE_FILENAMES
-
-
-def compute_isco(chi_bh):
-    '''
-    This function takes as input the aligned spin component of the BH and
-    returns the innermost stable circular orbit radius normalized by the mass
-    of the BH.
-    '''
-    if not np.all([np.abs(chi_bh) <= 1.0]):
-        raise ValueError('|chi1| must be less than 1.0')
-    Z1 = 1.0 + ((1.0 - chi_bh**2)**(1./3.))*((1 + chi_bh)**(1./3.) +
-                                             (1 - chi_bh)**(1./3.))
-    Z2 = np.sqrt(3*chi_bh**2 + Z1**2)
-    r_isco = 3 + Z2 - np.sign(chi_bh) * np.sqrt((3 - Z1)*(3 + Z1 + 2*Z2))
-    return r_isco
-
-
-def _lalsim_neutron_star_radius(m, max_mass, fam):
-    '''Return neutron star radius in meters'''
-    if m > max_mass:
-        return m * 1500  # 1 solar mass = 1500m
-    else:
-        try:
-            return lalsim.SimNeutronStarRadius(m * lal.MSUN_SI, fam)
-        except RuntimeError:
-            # FIXME handle RuntimeError for edge cases
-            # Raised if m is close to max_mass
-            # GSL function failed: interpolation error (errnum=1)
-            # XLAL Error - <GSL function> (interp.c:150): Generic failure
-            return m * 1500
-
-
-def _r_ns_from_lal_simulation(m_ns, eosname):
-    eos = lalsim.SimNeutronStarEOSByName(eosname)
-    fam = lalsim.CreateSimNeutronStarFamily(eos)
-    max_mass = lalsim.SimNeutronStarMaximumMass(fam)/c.M_sun.value
-    try:
-        iter(m_ns)
-        R_ns = np.array([_lalsim_neutron_star_radius(m, max_mass, fam)
-                        for m in m_ns])
-    except TypeError:
-        R_ns = _lalsim_neutron_star_radius(m_ns, max_mass, fam)
-    return R_ns, max_mass
-
-
-def _compactness_baryon_mass(m_ns, r_ns):
-    C_ns = c.G * m_ns * c.M_sun/(r_ns * u.m * c.c**2)
-    C_ns = C_ns.value
-
-    d1 = 0.619
-    d2 = 0.1359
-    BE = (d1*C_ns + d2*C_ns*C_ns) * m_ns  # arXiv:1601.06083 (Eq: 21)
-    m2_b = m_ns + BE  # Baryonic mass - Gravitational mass = Binding Energy
-    return [C_ns, m2_b]
-
-
-def computeCompactness(M_ns, eosname='2H', R_ns=None,
-                       max_mass=2.834648092299807):
-    '''
-    Return the neutron star compactness as a function of mass
-    and equation of state or radius
-
-    Parameters
-    ----------
-    M_ns : array_like
-        Neutron star mass in solar masses
-    eosname : str or interp1d
-        Neutron star equation of state to be used
-    R_ns : array_like
-        Neutron star radius.
-    max_mass : float
-        Maximum mass of neutron star.
-
-    Returns
-    -------
-    [C_ns, m2_b, max_mass]
-        Compactness, baryon mass and maximum neutron star mass
-        in solar masses.
-
-    Notes
-    -----
-    The radius and maximum mass of the neutron star is
-    inferred based on the equation of state supplied.
-    Supply explicitly if `eosname=None`.
-
-    Examples
-    --------
-    >>> computeCompactness(2.8)
-    [array(0.298), array(3.354), 2.834]
-    >>> computeDiskMass.computeCompactness(2.9, eosname='AP4')
-    [0.5, 0.0, 2.212]
-    >>> m_ns = np.array([1.1, 1.2, 1.3])
-    >>> computeDiskMass.computeCompactness(m_ns, eosname='AP4')
-    [array([0.141, 0.154, 0.167]), array([1.199, 1.318, 1.439]), 2.212]
-    >>> computeCompactness(2.1, R_ns=16000, eosname=None, max_mass=2.5)
-    [0.193, 2.362, 2.5]
-    '''
-    if R_ns:
-        C_ns, m2_b = _compactness_baryon_mass(M_ns, R_ns)
-    elif isinstance(eosname, interp1d):
-        # find R as a function of M
-        R_ns = eosname(M_ns)
-        C_ns, m2_b = _compactness_baryon_mass(M_ns, R_ns)
-    elif eosname != '2H':
-        # infer radius and maximum mass based on lalsimulation EoS
-        R_ns, max_mass = _r_ns_from_lal_simulation(M_ns, eosname)
-        C_ns, m2_b = _compactness_baryon_mass(M_ns, R_ns)
-    else:
-        with open(PACKAGE_FILENAMES['equil_2H.dat'], 'rb') as f:
-            M_g, M_b, Compactness = np.loadtxt(f, unpack=True)
-        max_mass = 2.834648092299807
-        s = UnivariateSpline(M_g, Compactness, k=5)
-        s_b = UnivariateSpline(M_g, M_b, k=5)
-        C_ns = s(M_ns)
-        m2_b = s_b(M_ns)
-    try:
-        C_ns[M_ns > max_mass] = 0.5  # BH compactness set to 0.5
-        m2_b[M_ns > max_mass] = 0.0  # BH baryon mass set to 0.0
-    except TypeError:  # if C_ns is not an array
-        if M_ns > max_mass:
-            C_ns = 0.5
-            m2_b = 0.0
-    return [C_ns, m2_b, max_mass]
-
-
-'''
-For Newtonian: Obtained from arXiv 1807.00011
-alpha = 0.406
-beta = 0.139
-gamma = 0.255
-delta = 1.761
-
-For Kerr: Obtained from private message from F. Foucart
-alpha = 0.24037857
-beta = 0.15184471
-gamma = 0.35607169
-delta = 1.81491784
-'''
-
-
-def xi_implicit(xi, kappa, chi1, eta):
-    xi_implicit = 3*(xi**2 - 2*kappa*xi + kappa**2*chi1**2)
-    xi_implicit /= (xi**2 - 3*kappa*xi + 2*chi1*np.sqrt(kappa**3*xi))
-    xi_implicit -= eta*xi**3
-    return xi_implicit
-
-
-def computeDiskMass(m1, m2, chi1, chi2, eosname='2H', kerr=False,
-                    R_ns=None, max_mass=None):
-    """
-    This function computes the remnant disk mass after the coalescence using
-    the equation (4) arXiv 1807.00011.
-
-    Parameters
-    ----------
-    m1, m2 : array_like
-        primary and secondary mass(es)
-    chi1, chi2 : array_like
-        primary and secondary spin(s)
-    eosname : str
-        Name of the equation of state to be used. `AP4`
-        `None` when supplying `R_ns`.
-    kerr : bool
-        Supply to use the relativistic tidal parameter. See Fishbone (1971).
-    R_ns : float
-        Radius of the secondary, assuming it is a neutron star.
-    max_mass : float
-        Maximum mass of a neutron star. To be supplied if not supplying EoS.
-
-    Example
-    -------
-    >>> computeDiskMass(5.0, 2.0, 0.99, 0.)
-    0.6321412881595185
-    >>> m1 = np.array([5., 6., 7.])
-    >>> m2 = np.array([1.0, 1.2, 1.6])
-    >>> chi1 = np.zeros(3)
-    >>> chi2 = np.zeros(3)
-    >>> computeDiskMass(m1, m2, chi1, chi2)
-    array([0.12833991, 0.05054819, 0.])
-    >>> computeDiskMass(m1, m2, chi1, chi2, eosname='AP4')
-    array([0.00851525, 0., 0.])
-    >>> max_mass = 3.0  # in m_sun
-    >>> r_ns = 15000.  # in meters
-    >>> computeDiskMass(m1, m2, chi1, chi2,
-    ...                 R_ns=r_ns, max_mass=max_mass, eosname=None)
-    array([0.12265712, 0.04272054, 0.])
-    >>> # m1=2.0, m2=2.0 is a BNS event assuming 2H EOS
-    >>> # DiskMass == 1.0 is a ad hoc value assigned for BNS events
-    >>> masses_spins = np.array([2.0, 2.0, 0., 0.])
-    >>> computeDiskMass(masses_spins[0], masses_spins[1],
-    ...                 masses_spins[2], masses_spins[3], eosname="2H")
-    1.0
-    >>> masses_spins = np.array([5.0, 2.0, 0.99, 0.])
-    >>> computeDiskMass(masses_spins[0], masses_spins[1],
-    ...                 masses_spins[2], masses_spins[3], eosname="2H")
-    0.6321412881595185
-
-    Notes
-    -----
-    The primary mass, by convention, is larger one. If arrays are supplied,
-    `m1`, `m2`, `chi1`, `chi1` should be of the same size.
-    """
-    try:
-        _ = iter(m1)
-        assert m1.size == m2.size == chi1.size == chi2.size, \
-            "masses and spins must have the same dimensions"
-        # Making sure that the supplied m1 >= m2 ##
-        largerMass1 = m1 >= m2
-        largerMass2 = m2 > m1
-        m_primary = np.zeros_like(m1)
-        m_secondary = np.zeros_like(m2)
-        chi_primary = np.zeros_like(chi1)
-        chi_secondary = np.zeros_like(chi2)
-
-        m_primary[largerMass1] = m1[largerMass1]
-        m_primary[~largerMass1] = m2[largerMass2]
-        m_secondary[~largerMass2] = m2[~largerMass2]
-        m_secondary[largerMass2] = m1[~largerMass1]
-
-        chi_primary[largerMass1] = chi1[largerMass1]
-        chi_primary[~largerMass1] = chi2[~largerMass1]
-        chi_secondary[~largerMass2] = chi2[~largerMass2]
-        chi_secondary[largerMass2] = chi1[~largerMass1]
-    except TypeError:
-        if m1 >= m2:
-            m_primary = m1
-            m_secondary = m2
-            chi_primary = chi1
-            chi_secondary = chi2
-        else:
-            m_primary = m2
-            m_secondary = m1
-            chi_primary = chi2
-            chi_secondary = chi1
-
-    [C_ns, m2_b, max_mass] = computeCompactness(m_secondary, eosname=eosname,
-                                                R_ns=R_ns, max_mass=max_mass)
-
-    eta = m_primary*m_secondary/(m_primary + m_secondary)**2
-    BBH = m_secondary > max_mass
-    BNS = m_primary < max_mass
-    # FIXME
-    if type(BNS) != np.ndarray:
-        if BNS or BBH:
-            return float(not (BBH) or BNS)
-
-    if not kerr:
-        alpha = 0.406
-        beta = 0.139
-        gamma = 0.255
-        delta = 1.761
-        firstTerm = alpha*(1 - 2*C_ns)/(eta**(1/3))
-        secondTerm = beta*compute_isco(chi1)*C_ns/eta
-        thirdTerm = gamma
-    else:
-        alpha = 0.24037857
-        beta = 0.15184471
-        gamma = 0.35607169
-        delta = 1.81491784
-        kappa = (m_primary/m_secondary)*C_ns
-        try:
-            Num = len(kappa)
-            xi = fsolve(xi_implicit, 100*np.ones(Num), args=(kappa, chi1, eta))
-        except TypeError:
-            xi = fsolve(xi_implicit, 100, args=(kappa, chi1, eta))
-
-        firstTerm = alpha*xi*(1 - 2*C_ns)
-        secondTerm = beta*compute_isco(chi1)*C_ns/eta
-        thirdTerm = gamma
-    combinedTerms = firstTerm - secondTerm + thirdTerm
-
-    if hasattr(combinedTerms, 'ndim') and combinedTerms.ndim >= 1:
-        lessthanzero = combinedTerms < 0.0
-        combinedTerms[lessthanzero] = 0.0
-    else:
-        combinedTerms = 0 if combinedTerms < 0 else combinedTerms
-    M_rem = (combinedTerms**delta)*m2_b
-    if type(BNS) == np.ndarray:
-        M_rem[BBH] = 0.0  # BBH is always EM-Dark
-        M_rem[BNS] = 1.0  # Ad hoc value, assuming BNS is always EM-Bright
-    return M_rem
+import numpy as np
+import astropy.units as u
+import astropy.constants as c
+from scipy.optimize import fsolve
+from scipy.interpolate import UnivariateSpline, interp1d
+
+import lal
+import lalsimulation as lalsim
+
+from .data import PACKAGE_FILENAMES
+
+
+def compute_isco(chi_bh):
+    '''
+    This function takes as input the aligned spin component of the BH and
+    returns the innermost stable circular orbit radius normalized by the mass
+    of the BH.
+    '''
+    if not np.all([np.abs(chi_bh) <= 1.0]):
+        raise ValueError('|chi1| must be less than 1.0')
+    Z1 = 1.0 + ((1.0 - chi_bh**2)**(1./3.))*((1 + chi_bh)**(1./3.) +
+                                             (1 - chi_bh)**(1./3.))
+    Z2 = np.sqrt(3*chi_bh**2 + Z1**2)
+    r_isco = 3 + Z2 - np.sign(chi_bh) * np.sqrt((3 - Z1)*(3 + Z1 + 2*Z2))
+    return r_isco
+
+
+def _lalsim_neutron_star_radius(m, max_mass, fam):
+    '''Return neutron star radius in meters'''
+    if m > max_mass:
+        return m * 1500  # 1 solar mass = 1500m
+    else:
+        try:
+            return lalsim.SimNeutronStarRadius(m * lal.MSUN_SI, fam)
+        except RuntimeError:
+            # FIXME handle RuntimeError for edge cases
+            # Raised if m is close to max_mass
+            # GSL function failed: interpolation error (errnum=1)
+            # XLAL Error - <GSL function> (interp.c:150): Generic failure
+            return m * 1500
+
+
+def _r_ns_from_lal_simulation(m_ns, eosname):
+    eos = lalsim.SimNeutronStarEOSByName(eosname)
+    fam = lalsim.CreateSimNeutronStarFamily(eos)
+    max_mass = lalsim.SimNeutronStarMaximumMass(fam)/c.M_sun.value
+    try:
+        iter(m_ns)
+        R_ns = np.array([_lalsim_neutron_star_radius(m, max_mass, fam)
+                        for m in m_ns])
+    except TypeError:
+        R_ns = _lalsim_neutron_star_radius(m_ns, max_mass, fam)
+    return R_ns, max_mass
+
+
+def _compactness_baryon_mass(m_ns, r_ns):
+    C_ns = c.G * m_ns * c.M_sun/(r_ns * u.m * c.c**2)
+    C_ns = C_ns.value
+
+    d1 = 0.619
+    d2 = 0.1359
+    BE = (d1*C_ns + d2*C_ns*C_ns) * m_ns  # arXiv:1601.06083 (Eq: 21)
+    m2_b = m_ns + BE  # Baryonic mass - Gravitational mass = Binding Energy
+    return [C_ns, m2_b]
+
+
+def computeCompactness(M_ns, eosname='2H', R_ns=None,
+                       max_mass=2.834648092299807):
+    '''
+    Return the neutron star compactness as a function of mass
+    and equation of state or radius
+
+    Parameters
+    ----------
+    M_ns : array_like
+        Neutron star mass in solar masses
+    eosname : str or interp1d
+        Neutron star equation of state to be used
+    R_ns : array_like
+        Neutron star radius in m.
+    max_mass : float
+        Maximum mass of neutron star.
+
+    Returns
+    -------
+    [C_ns, m2_b, max_mass]
+        Compactness, baryon mass and maximum neutron star mass
+        in solar masses.
+
+    Notes
+    -----
+    The radius and maximum mass of the neutron star is
+    inferred based on the equation of state supplied.
+    Supply explicitly if `eosname=None`.
+
+    Examples
+    --------
+    >>> computeCompactness(2.8)
+    [array(0.298), array(3.354), 2.834]
+    >>> computeDiskMass.computeCompactness(2.9, eosname='AP4')
+    [0.5, 0.0, 2.212]
+    >>> m_ns = np.array([1.1, 1.2, 1.3])
+    >>> computeDiskMass.computeCompactness(m_ns, eosname='AP4')
+    [array([0.141, 0.154, 0.167]), array([1.199, 1.318, 1.439]), 2.212]
+    >>> computeCompactness(2.1, R_ns=16000, eosname=None, max_mass=2.5)
+    [0.193, 2.362, 2.5]
+    '''
+    if R_ns:
+        C_ns, m2_b = _compactness_baryon_mass(M_ns, R_ns)
+    elif isinstance(eosname, interp1d):
+        # find R as a function of M
+        R_ns = eosname(M_ns)
+        C_ns, m2_b = _compactness_baryon_mass(M_ns, R_ns)
+    elif eosname != '2H':
+        # infer radius and maximum mass based on lalsimulation EoS
+        R_ns, max_mass = _r_ns_from_lal_simulation(M_ns, eosname)
+        C_ns, m2_b = _compactness_baryon_mass(M_ns, R_ns)
+    else:
+        with open(PACKAGE_FILENAMES['equil_2H.dat'], 'rb') as f:
+            M_g, M_b, Compactness = np.loadtxt(f, unpack=True)
+        max_mass = 2.834648092299807
+        s = UnivariateSpline(M_g, Compactness, k=5)
+        s_b = UnivariateSpline(M_g, M_b, k=5)
+        C_ns = s(M_ns)
+        m2_b = s_b(M_ns)
+    try:
+        C_ns[M_ns > max_mass] = 0.5  # BH compactness set to 0.5
+        m2_b[M_ns > max_mass] = 0.0  # BH baryon mass set to 0.0
+    except TypeError:  # if C_ns is not an array
+        if M_ns > max_mass:
+            C_ns = 0.5
+            m2_b = 0.0
+    return [C_ns, m2_b, max_mass]
+
+
+'''
+For Newtonian: Obtained from arXiv 1807.00011
+alpha = 0.406
+beta = 0.139
+gamma = 0.255
+delta = 1.761
+
+For Kerr: Obtained from private message from F. Foucart
+alpha = 0.24037857
+beta = 0.15184471
+gamma = 0.35607169
+delta = 1.81491784
+'''
+
+
+def xi_implicit(xi, kappa, chi1, eta):
+    xi_implicit = 3*(xi**2 - 2*kappa*xi + kappa**2*chi1**2)
+    xi_implicit /= (xi**2 - 3*kappa*xi + 2*chi1*np.sqrt(kappa**3*xi))
+    xi_implicit -= eta*xi**3
+    return xi_implicit
+
+
+def computeDiskMass(m1, m2, chi1, chi2, eosname='2H', kerr=False,
+                    R_ns=None, max_mass=None):
+    """
+    This function computes the remnant disk mass after the coalescence using
+    the equation (4) arXiv 1807.00011.
+
+    Parameters
+    ----------
+    m1, m2 : array_like
+        primary and secondary mass(es)
+    chi1, chi2 : array_like
+        primary and secondary spin(s)
+    eosname : str
+        Name of the equation of state to be used. `AP4`
+        `None` when supplying `R_ns`.
+    kerr : bool
+        Supply to use the relativistic tidal parameter. See Fishbone (1971).
+    R_ns : float
+        Radius of the secondary in m, assuming it is a neutron star.
+    max_mass : float
+        Maximum mass of a neutron star. To be supplied if not supplying EoS.
+
+    Example
+    -------
+    >>> computeDiskMass(5.0, 2.0, 0.99, 0.)
+    0.6321412881595185
+    >>> m1 = np.array([5., 6., 7.])
+    >>> m2 = np.array([1.0, 1.2, 1.6])
+    >>> chi1 = np.zeros(3)
+    >>> chi2 = np.zeros(3)
+    >>> computeDiskMass(m1, m2, chi1, chi2)
+    array([0.12833991, 0.05054819, 0.])
+    >>> computeDiskMass(m1, m2, chi1, chi2, eosname='AP4')
+    array([0.00851525, 0., 0.])
+    >>> max_mass = 3.0  # in m_sun
+    >>> r_ns = 15000.  # in meters
+    >>> computeDiskMass(m1, m2, chi1, chi2,
+    ...                 R_ns=r_ns, max_mass=max_mass, eosname=None)
+    array([0.12265712, 0.04272054, 0.])
+    >>> # m1=2.0, m2=2.0 is a BNS event assuming 2H EOS
+    >>> # DiskMass == 1.0 is a ad hoc value assigned for BNS events
+    >>> masses_spins = np.array([2.0, 2.0, 0., 0.])
+    >>> computeDiskMass(masses_spins[0], masses_spins[1],
+    ...                 masses_spins[2], masses_spins[3], eosname="2H")
+    1.0
+    >>> masses_spins = np.array([5.0, 2.0, 0.99, 0.])
+    >>> computeDiskMass(masses_spins[0], masses_spins[1],
+    ...                 masses_spins[2], masses_spins[3], eosname="2H")
+    0.6321412881595185
+
+    Notes
+    -----
+    The primary mass, by convention, is larger one. If arrays are supplied,
+    `m1`, `m2`, `chi1`, `chi1` should be of the same size.
+    """
+    try:
+        _ = iter(m1)
+        assert m1.size == m2.size == chi1.size == chi2.size, \
+            "masses and spins must have the same dimensions"
+        # Making sure that the supplied m1 >= m2 ##
+        largerMass1 = m1 >= m2
+        largerMass2 = m2 > m1
+        m_primary = np.zeros_like(m1)
+        m_secondary = np.zeros_like(m2)
+        chi_primary = np.zeros_like(chi1)
+        chi_secondary = np.zeros_like(chi2)
+
+        m_primary[largerMass1] = m1[largerMass1]
+        m_primary[~largerMass1] = m2[largerMass2]
+        m_secondary[~largerMass2] = m2[~largerMass2]
+        m_secondary[largerMass2] = m1[~largerMass1]
+
+        chi_primary[largerMass1] = chi1[largerMass1]
+        chi_primary[~largerMass1] = chi2[~largerMass1]
+        chi_secondary[~largerMass2] = chi2[~largerMass2]
+        chi_secondary[largerMass2] = chi1[~largerMass1]
+    except TypeError:
+        if m1 >= m2:
+            m_primary = m1
+            m_secondary = m2
+            chi_primary = chi1
+            chi_secondary = chi2
+        else:
+            m_primary = m2
+            m_secondary = m1
+            chi_primary = chi2
+            chi_secondary = chi1
+
+    [C_ns, m2_b, max_mass] = computeCompactness(m_secondary, eosname=eosname,
+                                                R_ns=R_ns, max_mass=max_mass)
+
+    eta = m_primary*m_secondary/(m_primary + m_secondary)**2
+    BBH = m_secondary > max_mass
+    BNS = m_primary < max_mass
+    # FIXME
+    if type(BNS) != np.ndarray:
+        if BNS or BBH:
+            return float(not (BBH) or BNS)
+
+    if not kerr:
+        alpha = 0.406
+        beta = 0.139
+        gamma = 0.255
+        delta = 1.761
+        firstTerm = alpha*(1 - 2*C_ns)/(eta**(1/3))
+        secondTerm = beta*compute_isco(chi1)*C_ns/eta
+        thirdTerm = gamma
+    else:
+        alpha = 0.24037857
+        beta = 0.15184471
+        gamma = 0.35607169
+        delta = 1.81491784
+        kappa = (m_primary/m_secondary)*C_ns
+        try:
+            Num = len(kappa)
+            xi = fsolve(xi_implicit, 100*np.ones(Num), args=(kappa, chi1, eta))
+        except TypeError:
+            xi = fsolve(xi_implicit, 100, args=(kappa, chi1, eta))
+
+        firstTerm = alpha*xi*(1 - 2*C_ns)
+        secondTerm = beta*compute_isco(chi1)*C_ns/eta
+        thirdTerm = gamma
+    combinedTerms = firstTerm - secondTerm + thirdTerm
+
+    if hasattr(combinedTerms, 'ndim') and combinedTerms.ndim >= 1:
+        lessthanzero = combinedTerms < 0.0
+        combinedTerms[lessthanzero] = 0.0
+    else:
+        combinedTerms = 0 if combinedTerms < 0 else combinedTerms
+    M_rem = (combinedTerms**delta)*m2_b
+    if type(BNS) == np.ndarray:
+        M_rem[BBH] = 0.0  # BBH is always EM-Dark
+        M_rem[BNS] = 1.0  # Ad hoc value, assuming BNS is always EM-Bright
+    return M_rem
```

### Comparing `ligo_em_bright-1.1.3/ligo/em_bright/dag_writer.py` & `ligo_em_bright-1.1.4/ligo/em_bright/dag_writer.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,381 +1,381 @@
-# Copyright(C) 2018-2022 Shaon Ghosh, Deep Chatterjee, Sushant Sharma Chaudhary
-#
-# This program is free software; you can redistribute it and/or modify it
-# under the terms of the GNU General Public License as published by the
-# Free Software Foundation; either version 2 of the License, or (at your
-# option) any later version.
-#
-# This program is distributed in the hope that it will be useful, but
-# WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU General
-# Public License for more details.
-#
-# You should have received a copy of the GNU General Public License along
-# with this program; if not, write to the Free Software Foundation, Inc.,
-# 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA.
-
-
-import os
-import re
-import shutil
-
-from argparse import ArgumentParser
-from configparser import ConfigParser
-from glob import glob
-
-from .data import EOS_BAYES_FACTORS
-
-try:
-    import htcondor
-    from htcondor import dags
-    _HTCONDOR_INSTALLED = True
-except ModuleNotFoundError:
-    _HTCONDOR_INSTALLED = False
-    import warnings
-    warnings.warn(
-        "HTCondor python bindings need to be installed to use this script. "
-        "This script is only used in training. When training new classifiers, "
-        "create a developmental version by cloning the git repository, "
-        "and installing from the lock file."
-    )
-
-
-def _add_common_workflow(condor_dag, args, common_submit_dict):
-    config = ConfigParser()
-    config.read(args.config)
-    config_path = os.path.abspath(args.config)
-    abs_work_dir = os.path.abspath(args.work_dir)
-    file_dir = args.file_dir
-    # Get injection directory
-    inj_file_pattern = config.get('core',
-                                  'inj_file_pattern')
-    sqlite_run_tag = config.get('core',
-                                'sqlite_run_tag')
-
-    # Get input and output file names prefixes
-    em_bright_extract_prefix = config.get('output_filenames',
-                                          'em_bright_extract_prefix')
-    em_bright_extract_suffix = config.get('output_filenames',
-                                          'em_bright_extract_suffix')
-    em_bright_join_prefix = config.get('output_filenames',
-                                       'em_bright_join_prefix')
-    em_bright_join_suffix = config.get('output_filenames',
-                                       'em_bright_join_suffix')
-    # Get executable names
-    em_bright_extract_executable = config.get('executables',
-                                              'em_bright_extract')
-    em_bright_join_executable = config.get('executables',
-                                           'em_bright_join')
-
-    # Define the executable arguments association
-    exec_arg_assoc = {
-        em_bright_extract_executable:
-            " --input $(macroinput) --output $(macrooutput)",
-        em_bright_join_executable:
-            " --input $(macroinput) --config $(macroconfig)"
-            " --output $(macrooutput)"
-    }
-    # create a dictionary of Submit instances
-    condor_sub_dict = dict.fromkeys(exec_arg_assoc)
-    # create all sub files
-
-    for exect, arg_sub in exec_arg_assoc.items():
-        common_submit_dict["executable"] = exect
-        common_submit_dict["arguments"] = arg_sub
-        condor_sub_dict[exect] = htcondor.Submit(
-            common_submit_dict)
-    # Creating list of sqlite files to create the dag
-    inj_list = glob(
-        os.path.join(
-            os.path.abspath(file_dir), inj_file_pattern
-        )
-    )
-
-    # get vars for em_bright_extract layer
-    em_bright_extract_vars = []
-    for idx, injFilename in enumerate(inj_list):
-        match = re.search(sqlite_run_tag, os.path.basename(injFilename))
-        if match is None:
-            continue
-        prefix, startT, duration = match.groups()
-        # filename for INJCOINC files
-        output_fname = \
-            em_bright_extract_prefix + \
-            prefix + '-' + startT + '-' + duration + em_bright_extract_suffix
-        em_bright_extract_vars.append(
-            dict(
-                macroinput=injFilename,
-                macrooutput=output_fname
-            )
-        )
-    em_bright_extract_layer = condor_dag.layer(
-        name=em_bright_extract_executable,
-        submit_description=condor_sub_dict[em_bright_extract_executable],
-        vars=em_bright_extract_vars
-    )
-    # output for JOIN
-    join_output = \
-        em_bright_join_prefix + '-' + startT + '-' + \
-        duration + em_bright_join_suffix
-    join_output = os.path.join(abs_work_dir, join_output)
-
-    em_bright_join_vars = [
-        dict(
-            macroinput=abs_work_dir,
-            macrooutput=join_output,
-            macroconfig=config_path
-        )
-    ]
-    em_bright_join_layer = em_bright_extract_layer.child_layer(
-        name=em_bright_join_executable,
-        submit_description=condor_sub_dict[em_bright_join_executable],
-        vars=em_bright_join_vars
-    )
-    join_output_dict = {
-        "output": join_output,
-        "startT": startT,
-        "duration": duration
-    }
-    return em_bright_join_layer, join_output_dict
-
-
-def _add_knn_workflow(em_bright_join_layer, args,
-                      common_submit_dict,
-                      join_output_dict):
-    config = ConfigParser()
-    config.read(args.config)
-    config_path = os.path.abspath(args.config)
-    abs_work_dir = os.path.abspath(args.work_dir)
-
-    em_bright_categorize_prefix = config.get('output_filenames',
-                                             'em_bright_categorize_prefix')
-    em_bright_categorize_suffix = config.get('output_filenames',
-                                             'em_bright_categorize_suffix')
-    em_bright_train_prefix = config.get('output_filenames',
-                                        'em_bright_train_prefix')
-    em_bright_train_suffix = config.get('output_filenames',
-                                        'em_bright_train_suffix')
-    em_bright_categorize_executable = config.get('executables',
-                                                 'em_bright_categorize')
-    em_bright_train_executable = config.get('executables',
-                                            'em_bright_train')
-    em_bright_paramater_sweep_plot_executable = config.get(
-            'executables', 'em_bright_create_param_sweep_plot'
-    )
-    exec_arg_assoc = {
-        em_bright_train_executable:
-            " --input $(macroinput) --config $(macroconfig) "
-            "--output $(macrooutput) --param-sweep-plot-prefix $(macroeos)",
-        em_bright_paramater_sweep_plot_executable:
-            " --input $(macroinput) --config $(macroconfig)"
-            " --verbose",
-        em_bright_categorize_executable:
-            " --input $(macroinput) --output $(macrooutput)"
-            " --eosname $(macroeos) "
-    }
-    condor_sub_dict = dict.fromkeys(exec_arg_assoc)
-
-    for exect, arg_sub in exec_arg_assoc.items():
-        common_submit_dict["executable"] = exect
-        common_submit_dict["arguments"] = arg_sub
-        condor_sub_dict[exect] = htcondor.Submit(
-            common_submit_dict)
-
-    # input and output for CATEGORIZE/TRAIN
-    em_bright_categorize_vars = list()
-    em_bright_train_vars = list()
-    categorize_input = join_output_dict["output"]
-
-    for em_bright_eos in EOS_BAYES_FACTORS:
-        categorize_output = \
-            em_bright_categorize_prefix + '-' + join_output_dict["startT"] + \
-            '-' + join_output_dict["duration"] + '-' + em_bright_eos + \
-            em_bright_categorize_suffix
-        categorize_output = os.path.join(abs_work_dir, categorize_output)
-
-        train_output = \
-            em_bright_train_prefix + '-' + join_output_dict["startT"] + \
-            '-' + join_output_dict["duration"] + \
-            '-' + em_bright_eos + em_bright_train_suffix
-        train_output = os.path.join(abs_work_dir, train_output)
-
-        em_bright_categorize_vars.append(
-            dict(
-                macroinput=categorize_input,
-                macrooutput=categorize_output,
-                macroeos=em_bright_eos,
-            )
-        )
-        em_bright_train_vars.append(
-                dict(
-                    macroinput=categorize_output,
-                    macrooutput=train_output,
-                    macroconfig=config_path,
-                    macroeos=em_bright_eos
-                )
-            )
-
-    em_bright_categorize_layer = em_bright_join_layer.child_layer(
-        name=em_bright_categorize_executable,
-        submit_description=condor_sub_dict[em_bright_categorize_executable],
-        vars=em_bright_categorize_vars
-    )
-
-    em_bright_train_layer = em_bright_categorize_layer.child_layer(
-            name=em_bright_train_executable,
-            submit_description=condor_sub_dict[em_bright_train_executable],
-            vars=em_bright_train_vars
-        )
-
-    em_bright_param_sweep_layer = em_bright_train_layer.child_layer(  # noqa: F841,E501
-            name=em_bright_paramater_sweep_plot_executable,
-            submit_description=condor_sub_dict[
-                em_bright_paramater_sweep_plot_executable],
-            vars=[
-                dict(
-                    macroinput=abs_work_dir,
-                    macroconfig=config_path
-                )
-            ]
-        )
-
-
-def _add_massgap_workflow(em_bright_join_layer, args,
-                          common_submit_dict,
-                          join_output_dict):
-    config = ConfigParser()
-    config.read(args.config)
-    config_path = os.path.abspath(args.config)
-    abs_work_dir = os.path.abspath(args.work_dir)
-
-    em_bright_categorize_prefix = config.get('output_filenames',
-                                             'em_bright_categorize_prefix')
-    em_bright_categorize_suffix = config.get('output_filenames',
-                                             'em_bright_categorize_suffix')
-    em_bright_train_suffix = config.get('output_filenames',
-                                        'em_bright_train_suffix')
-    em_bright_categorize_executable = config.get('executables',
-                                                 'em_bright_categorize')
-    em_bright_train_executable = config.get('executables',
-                                            'em_bright_train')
-    exec_arg_assoc = {
-        em_bright_categorize_executable:
-            " --input $(macroinput) --output $(macrooutput)"
-            " --mass-gap",
-        em_bright_train_executable:
-            " --input $(macroinput) --config $(macroconfig)"
-            " --output $(macrooutput) --mass-gap"
-    }
-    condor_sub_dict = dict.fromkeys(exec_arg_assoc)
-    for exect, arg_sub in exec_arg_assoc.items():
-        common_submit_dict["executable"] = exect
-        common_submit_dict["arguments"] = arg_sub
-        condor_sub_dict[exect] = htcondor.Submit(
-            common_submit_dict)
-
-    categorize_input = join_output_dict["output"]
-    categorize_output = \
-        em_bright_categorize_prefix + '-' + join_output_dict["startT"] + \
-        '-' + join_output_dict["duration"] + \
-        em_bright_categorize_suffix
-    categorize_output = os.path.join(abs_work_dir, categorize_output)
-
-    em_bright_categorize_vars = [
-            dict(
-                macroinput=categorize_input,
-                macrooutput=categorize_output,
-            )
-    ]
-    em_bright_categorize_layer = em_bright_join_layer.child_layer(
-        name=em_bright_categorize_executable,
-        submit_description=condor_sub_dict[em_bright_categorize_executable],
-        vars=em_bright_categorize_vars
-    )
-
-    train_output = "mass_gap" + \
-        em_bright_train_suffix
-    train_output = os.path.join(abs_work_dir, train_output)
-
-    em_bright_train_vars = [
-         dict(
-                macroinput=categorize_output,
-                macrooutput=train_output,
-                macroconfig=config_path,
-            )
-    ]
-    em_bright_categorize_layer.child_layer(
-            name=em_bright_train_executable,
-            submit_description=condor_sub_dict[em_bright_train_executable],
-            vars=em_bright_train_vars
-        )
-
-
-def main():
-    parser = ArgumentParser("Condor DAG writer for workflow")
-    parser.add_argument("-d", "--dagname", required=True,
-                        help="Name of the dag file. Placed under --work-dir")
-    parser.add_argument("-w", "--work-dir", required=True,
-                        help="Working directory to store data outputs")
-    parser.add_argument(
-        "-i", "--file-dir", required=True,
-        help="File containing input injection sqlite databases"
-    )
-    parser.add_argument("-c", "--config", required=True,
-                        help="Name of the config file")
-    parser.add_argument("-e", "--executables-dir", required=True,
-                        help="Directory containing executables")
-    parser.add_argument("--mass-gap", action='store_true',
-                        help="use --random_forest for Random Forest Mode")
-    args = parser.parse_args()
-
-    assert _HTCONDOR_INSTALLED, "HTCondor python bindings missing."
-
-    config = ConfigParser()
-    config.read(args.config)
-    # Get path for the work directory
-    if not os.path.exists(args.work_dir):
-        os.makedirs(args.work_dir)
-    abs_work_dir = os.path.abspath(args.work_dir)
-    accounting_group = config.get('core',
-                                  'accounting_group')
-    # changes made here
-    common_submit_dict = {
-            'universe': 'vanilla',
-            'request_disk': '1GB',
-            'output': '$(executable).stdout',
-            'error': '$(executable).stderr',
-            'log': '$(executable).log',
-            'accounting_group': accounting_group
-    }
-
-    condor_dag = dags.DAG()
-    join_layer, join_output_dict = _add_common_workflow(
-                                                condor_dag,
-                                                args,
-                                                common_submit_dict)
-    if not args.mass_gap:
-        _add_knn_workflow(join_layer, args,
-                          common_submit_dict,
-                          join_output_dict)
-    else:
-        _add_massgap_workflow(join_layer, args,
-                              common_submit_dict,
-                              join_output_dict)
-
-    print("DAG desription:\n", condor_dag.describe())
-    dags.write_dag(condor_dag, abs_work_dir,
-                   dag_file_name=args.dagname)
-
-    # FIXME Condor refuses to carry over env vars
-    # remove when solution is found
-    for exe in config['executables']:
-        src = os.path.join(args.executables_dir, exe)
-        dst = os.path.join(abs_work_dir, exe)
-        if os.path.lexists(dst):
-            os.remove(dst)
-        shutil.copy(src, dst)
-    print('{} is written in {}'.format(args.dagname, abs_work_dir))
-
-
-if __name__ == "__main__":
-    main()
+# Copyright(C) 2018-2022 Shaon Ghosh, Deep Chatterjee, Sushant Sharma Chaudhary
+#
+# This program is free software; you can redistribute it and/or modify it
+# under the terms of the GNU General Public License as published by the
+# Free Software Foundation; either version 2 of the License, or (at your
+# option) any later version.
+#
+# This program is distributed in the hope that it will be useful, but
+# WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU General
+# Public License for more details.
+#
+# You should have received a copy of the GNU General Public License along
+# with this program; if not, write to the Free Software Foundation, Inc.,
+# 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA.
+
+
+import os
+import re
+import shutil
+
+from argparse import ArgumentParser
+from configparser import ConfigParser
+from glob import glob
+
+from .data import EOS_BAYES_FACTORS
+
+try:
+    import htcondor
+    from htcondor import dags
+    _HTCONDOR_INSTALLED = True
+except ModuleNotFoundError:
+    _HTCONDOR_INSTALLED = False
+    import warnings
+    warnings.warn(
+        "HTCondor python bindings need to be installed to use this script. "
+        "This script is only used in training. When training new classifiers, "
+        "create a developmental version by cloning the git repository, "
+        "and installing from the lock file."
+    )
+
+
+def _add_common_workflow(condor_dag, args, common_submit_dict):
+    config = ConfigParser()
+    config.read(args.config)
+    config_path = os.path.abspath(args.config)
+    abs_work_dir = os.path.abspath(args.work_dir)
+    file_dir = args.file_dir
+    # Get injection directory
+    inj_file_pattern = config.get('core',
+                                  'inj_file_pattern')
+    sqlite_run_tag = config.get('core',
+                                'sqlite_run_tag')
+
+    # Get input and output file names prefixes
+    em_bright_extract_prefix = config.get('output_filenames',
+                                          'em_bright_extract_prefix')
+    em_bright_extract_suffix = config.get('output_filenames',
+                                          'em_bright_extract_suffix')
+    em_bright_join_prefix = config.get('output_filenames',
+                                       'em_bright_join_prefix')
+    em_bright_join_suffix = config.get('output_filenames',
+                                       'em_bright_join_suffix')
+    # Get executable names
+    em_bright_extract_executable = config.get('executables',
+                                              'em_bright_extract')
+    em_bright_join_executable = config.get('executables',
+                                           'em_bright_join')
+
+    # Define the executable arguments association
+    exec_arg_assoc = {
+        em_bright_extract_executable:
+            " --input $(macroinput) --output $(macrooutput)",
+        em_bright_join_executable:
+            " --input $(macroinput) --config $(macroconfig)"
+            " --output $(macrooutput)"
+    }
+    # create a dictionary of Submit instances
+    condor_sub_dict = dict.fromkeys(exec_arg_assoc)
+    # create all sub files
+
+    for exect, arg_sub in exec_arg_assoc.items():
+        common_submit_dict["executable"] = exect
+        common_submit_dict["arguments"] = arg_sub
+        condor_sub_dict[exect] = htcondor.Submit(
+            common_submit_dict)
+    # Creating list of sqlite files to create the dag
+    inj_list = glob(
+        os.path.join(
+            os.path.abspath(file_dir), inj_file_pattern
+        )
+    )
+
+    # get vars for em_bright_extract layer
+    em_bright_extract_vars = []
+    for idx, injFilename in enumerate(inj_list):
+        match = re.search(sqlite_run_tag, os.path.basename(injFilename))
+        if match is None:
+            continue
+        prefix, startT, duration = match.groups()
+        # filename for INJCOINC files
+        output_fname = \
+            em_bright_extract_prefix + \
+            prefix + '-' + startT + '-' + duration + em_bright_extract_suffix
+        em_bright_extract_vars.append(
+            dict(
+                macroinput=injFilename,
+                macrooutput=output_fname
+            )
+        )
+    em_bright_extract_layer = condor_dag.layer(
+        name=em_bright_extract_executable,
+        submit_description=condor_sub_dict[em_bright_extract_executable],
+        vars=em_bright_extract_vars
+    )
+    # output for JOIN
+    join_output = \
+        em_bright_join_prefix + '-' + startT + '-' + \
+        duration + em_bright_join_suffix
+    join_output = os.path.join(abs_work_dir, join_output)
+
+    em_bright_join_vars = [
+        dict(
+            macroinput=abs_work_dir,
+            macrooutput=join_output,
+            macroconfig=config_path
+        )
+    ]
+    em_bright_join_layer = em_bright_extract_layer.child_layer(
+        name=em_bright_join_executable,
+        submit_description=condor_sub_dict[em_bright_join_executable],
+        vars=em_bright_join_vars
+    )
+    join_output_dict = {
+        "output": join_output,
+        "startT": startT,
+        "duration": duration
+    }
+    return em_bright_join_layer, join_output_dict
+
+
+def _add_knn_workflow(em_bright_join_layer, args,
+                      common_submit_dict,
+                      join_output_dict):
+    config = ConfigParser()
+    config.read(args.config)
+    config_path = os.path.abspath(args.config)
+    abs_work_dir = os.path.abspath(args.work_dir)
+
+    em_bright_categorize_prefix = config.get('output_filenames',
+                                             'em_bright_categorize_prefix')
+    em_bright_categorize_suffix = config.get('output_filenames',
+                                             'em_bright_categorize_suffix')
+    em_bright_train_prefix = config.get('output_filenames',
+                                        'em_bright_train_prefix')
+    em_bright_train_suffix = config.get('output_filenames',
+                                        'em_bright_train_suffix')
+    em_bright_categorize_executable = config.get('executables',
+                                                 'em_bright_categorize')
+    em_bright_train_executable = config.get('executables',
+                                            'em_bright_train')
+    em_bright_paramater_sweep_plot_executable = config.get(
+            'executables', 'em_bright_create_param_sweep_plot'
+    )
+    exec_arg_assoc = {
+        em_bright_train_executable:
+            " --input $(macroinput) --config $(macroconfig) "
+            "--output $(macrooutput) --param-sweep-plot-prefix $(macroeos)",
+        em_bright_paramater_sweep_plot_executable:
+            " --input $(macroinput) --config $(macroconfig)"
+            " --verbose",
+        em_bright_categorize_executable:
+            " --input $(macroinput) --output $(macrooutput)"
+            " --eosname $(macroeos) "
+    }
+    condor_sub_dict = dict.fromkeys(exec_arg_assoc)
+
+    for exect, arg_sub in exec_arg_assoc.items():
+        common_submit_dict["executable"] = exect
+        common_submit_dict["arguments"] = arg_sub
+        condor_sub_dict[exect] = htcondor.Submit(
+            common_submit_dict)
+
+    # input and output for CATEGORIZE/TRAIN
+    em_bright_categorize_vars = list()
+    em_bright_train_vars = list()
+    categorize_input = join_output_dict["output"]
+
+    for em_bright_eos in EOS_BAYES_FACTORS:
+        categorize_output = \
+            em_bright_categorize_prefix + '-' + join_output_dict["startT"] + \
+            '-' + join_output_dict["duration"] + '-' + em_bright_eos + \
+            em_bright_categorize_suffix
+        categorize_output = os.path.join(abs_work_dir, categorize_output)
+
+        train_output = \
+            em_bright_train_prefix + '-' + join_output_dict["startT"] + \
+            '-' + join_output_dict["duration"] + \
+            '-' + em_bright_eos + em_bright_train_suffix
+        train_output = os.path.join(abs_work_dir, train_output)
+
+        em_bright_categorize_vars.append(
+            dict(
+                macroinput=categorize_input,
+                macrooutput=categorize_output,
+                macroeos=em_bright_eos,
+            )
+        )
+        em_bright_train_vars.append(
+                dict(
+                    macroinput=categorize_output,
+                    macrooutput=train_output,
+                    macroconfig=config_path,
+                    macroeos=em_bright_eos
+                )
+            )
+
+    em_bright_categorize_layer = em_bright_join_layer.child_layer(
+        name=em_bright_categorize_executable,
+        submit_description=condor_sub_dict[em_bright_categorize_executable],
+        vars=em_bright_categorize_vars
+    )
+
+    em_bright_train_layer = em_bright_categorize_layer.child_layer(
+            name=em_bright_train_executable,
+            submit_description=condor_sub_dict[em_bright_train_executable],
+            vars=em_bright_train_vars
+        )
+
+    em_bright_param_sweep_layer = em_bright_train_layer.child_layer(  # noqa: F841,E501
+            name=em_bright_paramater_sweep_plot_executable,
+            submit_description=condor_sub_dict[
+                em_bright_paramater_sweep_plot_executable],
+            vars=[
+                dict(
+                    macroinput=abs_work_dir,
+                    macroconfig=config_path
+                )
+            ]
+        )
+
+
+def _add_massgap_workflow(em_bright_join_layer, args,
+                          common_submit_dict,
+                          join_output_dict):
+    config = ConfigParser()
+    config.read(args.config)
+    config_path = os.path.abspath(args.config)
+    abs_work_dir = os.path.abspath(args.work_dir)
+
+    em_bright_categorize_prefix = config.get('output_filenames',
+                                             'em_bright_categorize_prefix')
+    em_bright_categorize_suffix = config.get('output_filenames',
+                                             'em_bright_categorize_suffix')
+    em_bright_train_suffix = config.get('output_filenames',
+                                        'em_bright_train_suffix')
+    em_bright_categorize_executable = config.get('executables',
+                                                 'em_bright_categorize')
+    em_bright_train_executable = config.get('executables',
+                                            'em_bright_train')
+    exec_arg_assoc = {
+        em_bright_categorize_executable:
+            " --input $(macroinput) --output $(macrooutput)"
+            " --mass-gap",
+        em_bright_train_executable:
+            " --input $(macroinput) --config $(macroconfig)"
+            " --output $(macrooutput) --mass-gap"
+    }
+    condor_sub_dict = dict.fromkeys(exec_arg_assoc)
+    for exect, arg_sub in exec_arg_assoc.items():
+        common_submit_dict["executable"] = exect
+        common_submit_dict["arguments"] = arg_sub
+        condor_sub_dict[exect] = htcondor.Submit(
+            common_submit_dict)
+
+    categorize_input = join_output_dict["output"]
+    categorize_output = \
+        em_bright_categorize_prefix + '-' + join_output_dict["startT"] + \
+        '-' + join_output_dict["duration"] + \
+        em_bright_categorize_suffix
+    categorize_output = os.path.join(abs_work_dir, categorize_output)
+
+    em_bright_categorize_vars = [
+            dict(
+                macroinput=categorize_input,
+                macrooutput=categorize_output,
+            )
+    ]
+    em_bright_categorize_layer = em_bright_join_layer.child_layer(
+        name=em_bright_categorize_executable,
+        submit_description=condor_sub_dict[em_bright_categorize_executable],
+        vars=em_bright_categorize_vars
+    )
+
+    train_output = "mass_gap" + \
+        em_bright_train_suffix
+    train_output = os.path.join(abs_work_dir, train_output)
+
+    em_bright_train_vars = [
+         dict(
+                macroinput=categorize_output,
+                macrooutput=train_output,
+                macroconfig=config_path,
+            )
+    ]
+    em_bright_categorize_layer.child_layer(
+            name=em_bright_train_executable,
+            submit_description=condor_sub_dict[em_bright_train_executable],
+            vars=em_bright_train_vars
+        )
+
+
+def main():
+    parser = ArgumentParser("Condor DAG writer for workflow")
+    parser.add_argument("-d", "--dagname", required=True,
+                        help="Name of the dag file. Placed under --work-dir")
+    parser.add_argument("-w", "--work-dir", required=True,
+                        help="Working directory to store data outputs")
+    parser.add_argument(
+        "-i", "--file-dir", required=True,
+        help="File containing input injection sqlite databases"
+    )
+    parser.add_argument("-c", "--config", required=True,
+                        help="Name of the config file")
+    parser.add_argument("-e", "--executables-dir", required=True,
+                        help="Directory containing executables")
+    parser.add_argument("--mass-gap", action='store_true',
+                        help="use --random_forest for Random Forest Mode")
+    args = parser.parse_args()
+
+    assert _HTCONDOR_INSTALLED, "HTCondor python bindings missing."
+
+    config = ConfigParser()
+    config.read(args.config)
+    # Get path for the work directory
+    if not os.path.exists(args.work_dir):
+        os.makedirs(args.work_dir)
+    abs_work_dir = os.path.abspath(args.work_dir)
+    accounting_group = config.get('core',
+                                  'accounting_group')
+    # changes made here
+    common_submit_dict = {
+            'universe': 'vanilla',
+            'request_disk': '1GB',
+            'output': '$(executable).stdout',
+            'error': '$(executable).stderr',
+            'log': '$(executable).log',
+            'accounting_group': accounting_group
+    }
+
+    condor_dag = dags.DAG()
+    join_layer, join_output_dict = _add_common_workflow(
+                                                condor_dag,
+                                                args,
+                                                common_submit_dict)
+    if not args.mass_gap:
+        _add_knn_workflow(join_layer, args,
+                          common_submit_dict,
+                          join_output_dict)
+    else:
+        _add_massgap_workflow(join_layer, args,
+                              common_submit_dict,
+                              join_output_dict)
+
+    print("DAG desription:\n", condor_dag.describe())
+    dags.write_dag(condor_dag, abs_work_dir,
+                   dag_file_name=args.dagname)
+
+    # FIXME Condor refuses to carry over env vars
+    # remove when solution is found
+    for exe in config['executables']:
+        src = os.path.join(args.executables_dir, exe)
+        dst = os.path.join(abs_work_dir, exe)
+        if os.path.lexists(dst):
+            os.remove(dst)
+        shutil.copy(src, dst)
+    print('{} is written in {}'.format(args.dagname, abs_work_dir))
+
+
+if __name__ == "__main__":
+    main()
```

### Comparing `ligo_em_bright-1.1.3/ligo/em_bright/em_bright.py` & `ligo_em_bright-1.1.4/ligo/em_bright/em_bright.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,237 +1,244 @@
-"""Module containing tools for EM-Bright classification of
-compact binaries using trained supervised classifier
-"""
-import h5py
-import numpy as np
-from scipy.interpolate import interp1d
-from astropy import cosmology, units as u
-
-from . import computeDiskMass, utils
-from .data import EOS_BAYES_FACTORS, PACKAGE_FILENAMES
-
-ALL_EOS_DRAWS = utils.load_eos_posterior()
-
-_classifiers = {
-    eos: utils._open_and_return_clfs(
-        PACKAGE_FILENAMES[f'{eos}.pickle']
-    )
-    for eos in EOS_BAYES_FACTORS
-}
-"""Classifiers keyed on EOS names. Order (clf_ns, clf_em)"""
-assert set(_classifiers) == set(EOS_BAYES_FACTORS), "Inconsistency in"
-" number of trained classifiers."
-
-_massgap_classifier = utils._open_and_return_clfs(
-        PACKAGE_FILENAMES['MASS_GAP.pickle']
-    )
-
-
-def mchirp(mass_1, mass_2):
-    return (mass_1 * mass_2)**(3./5.)/(mass_1 + mass_2)**(1./5.)
-
-
-def q(mass_1, mass_2):
-    return mass_2/mass_1 if mass_2 < mass_1 else mass_1/mass_2
-
-
-def source_classification(mass_1, mass_2, chi1, chi2, snr,
-                          ns_classifier=None,
-                          emb_classifier=None,
-                          massgap_classifier=None):
-    """
-    Computes ``HasNS``, ``HasRemnant``, and ``MassGap``
-    probabilities from point mass, spin and
-    signal to noise ratio estimates.
-
-    Parameters
-    ----------
-    mass_1 : float
-        primary mass
-    mass_2 : float
-        secondary mass
-    chi1 : float
-        dimensionless primary spin
-    chi2 : float
-        dimensionless secondary spin
-    snr : float
-        signal to noise ratio of the signal
-    ns_classifier : object, optional
-        pickled object for NS classification
-    emb_classifier : object, optional
-        pickled object for EM brightness classification
-    massgap_classifier : object, optional
-        pickled object for EM brightness classification
-
-    Returns
-    -------
-    tuple
-        (HasNS, HasRemnant, HasMassGap) predicted values.
-    Notes
-    -----
-    By default the classifiers, trained based
-    on different nuclear equations of state (EoSs)
-    are downloaded from the project page:
-    https://git.ligo.org/emfollow/em-properties/em-bright.
-    The methodology is described in arXiv:1911.00116.
-    The score from each classifier is weighted based on
-    the bayes factors of individual EoSs as mentioned in
-    Table I of arXiv:2104.08681.
-    However, if the trained classifiers are supplied
-    via ``ns_classifier`` and ``emb_classifier``,
-    the score is reported based on the classifier instead
-    of re-weighting the score.
-    Examples
-    --------
-    >>> from ligo.em_bright import em_bright
-    >>> em_bright.source_classification(2.0 ,1.0 ,0. ,0. ,10.0)
-    (1.0, 1.0, 0.0)
-    """
-    features = [[mass_1, mass_2, chi1, chi2, snr]]
-    try:
-        # custom classifiers supplied
-        return (
-            ns_classifier.predict_proba(features).T[1][0],
-            emb_classifier.predict_proba(features).T[1][0],
-            massgap_classifier.predict_proba(features).T[1][0]
-        )
-    except AttributeError as e:
-        msg, *_ = e.args
-        if msg != """'NoneType' object has no attribute 'predict_proba'""":
-            raise
-
-    reweighted_ns_score = reweighted_emb_score = 0.
-    for eosname, bayes_factor in EOS_BAYES_FACTORS.items():
-        ns_classifier, emb_classifier = _classifiers[eosname]
-        reweighted_ns_score += ns_classifier.predict_proba(
-            features).T[1][0] * bayes_factor
-        reweighted_emb_score += emb_classifier.predict_proba(
-            features).T[1][0] * bayes_factor
-    massgap_score = _massgap_classifier.predict_proba(features).T[1][0]
-    return reweighted_ns_score, reweighted_emb_score, massgap_score
-
-
-def get_redshifts(distances, N=10000):
-    """
-    Compute redshift using the Planck15 cosmology.
-
-    Parameters
-    ----------
-    distances: float or numpy.ndarray
-              distance(s) in Mpc
-
-    N : int, optional
-      Number of steps for the computation of the interpolation function
-
-    Example
-    -------
-    >>> distances = np.linspace(10, 100, 10)
-    >>> em_bright.get_redshifts(distances)
-    array([0.00225566, 0.00450357, 0.00674384, 0.00897655,
-           0.01120181, 0.0134197 , 0.01563032, 0.01783375
-           0.02003009, 0.02221941])
-
-    Notes
-    -----
-    This function accepts HDF5 posterior samples file and computes
-    redshift by interpolating the distance-redshift relation.
-    """
-    function = cosmology.Planck15.luminosity_distance
-    min_dist = np.min(distances)
-    max_dist = np.max(distances)
-    z_min = cosmology.z_at_value(func=function, fval=min_dist*u.Mpc)
-    z_max = cosmology.z_at_value(func=function, fval=max_dist*u.Mpc)
-    z_steps = np.linspace(z_min - (0.1*z_min), z_max + (0.1*z_max), N)
-    lum_dists = cosmology.Planck15.luminosity_distance(z_steps)
-    s = interp1d(lum_dists, z_steps)
-    redshifts = s(distances)
-    return redshifts
-
-
-def source_classification_pe(posterior_samples_file, threshold=3.0,
-                             num_eos_draws=None, eos_seed=None):
-    """
-    Compute ``HasNS``, ``HasRemnant``, and ``HasMassGap`` probabilities
-    from posterior samples.
-
-    Parameters
-    ----------
-    posterior_samples_file : str
-        Posterior samples file
-
-    threshold : float, optional
-        Maximum neutron star mass for `HasNS` computation
-
-    num_eos_draws : int
-        providing an int here runs eos marginalization
-        with the value determining how many eos's to draw
-
-    eos_seed : int
-        seed for random eos draws
-
-    Returns
-    -------
-    tuple
-        (HasNS, HasRemnant, HasMassGap) predicted values.
-
-
-    Examples
-    --------
-    >>> from ligo.em_bright import em_bright
-    >>> em_bright.source_classification_pe('posterior_samples.hdf5')
-    (1.0, 0.96, 0.0)
-    """
-    with h5py.File(posterior_samples_file, 'r') as data:
-        samples = data['posterior_samples'][()]
-
-    try:
-        mass_1, mass_2 = samples['mass_1_source'], samples['mass_2_source']
-    except ValueError:
-        lum_dist = samples['luminosity_distance']
-        redshifts = get_redshifts(lum_dist)
-        try:
-            mass_1, mass_2 = samples['mass_1'], samples['mass_2']
-            mass_1, mass_2 = mass_1/(1 + redshifts), mass_2/(1 + redshifts)
-        except ValueError:
-            chirp_mass, mass_ratio = samples['chirp_mass'], samples['mass_ratio']  # noqa:E501
-            chirp_mass = chirp_mass/(1 + redshifts)
-            mass_1 = chirp_mass * (1 + mass_ratio)**(1/5) * (mass_ratio)**(-3/5)  # noqa:E501
-            mass_2 = chirp_mass * (1 + mass_ratio)**(1/5) * (mass_ratio)**(2/5)
-
-    try:
-        a_1 = samples["spin_1z"]
-        a_2 = samples["spin_2z"]
-    except ValueError:
-        try:
-            a_1 = samples['a_1'] * np.cos(samples['tilt_1'])
-            a_2 = samples['a_2'] * np.cos(samples['tilt_2'])
-        except ValueError:
-            a_1, a_2 = np.zeros(len(mass_1)), np.zeros(len(mass_2))
-
-    if num_eos_draws:
-        np.random.seed(eos_seed)
-        prediction_nss, prediction_ems = [], []
-        for m1, m2, a1, a2 in zip(mass_1, mass_2, a_1, a_2):
-            rand_subset = np.random.choice(
-                len(ALL_EOS_DRAWS), num_eos_draws if num_eos_draws < len(ALL_EOS_DRAWS) else len(ALL_EOS_DRAWS))  # noqa:E501
-            subset_draws = ALL_EOS_DRAWS[rand_subset]
-            M, R = subset_draws['M'], subset_draws['R']
-            max_masses = np.max(M, axis=1)
-            f_M = [interp1d(m, r, bounds_error=False) for m, r in zip(M, R)]
-            for mass_radius_relation, max_mass in zip(f_M, max_masses):
-                M_rem = computeDiskMass.computeDiskMass(m1, m2, a1, a2, eosname=mass_radius_relation, max_mass=max_mass)  # noqa:E501
-                prediction_nss.append(1. if m2 <= max_mass else 0.)
-                prediction_ems.append(1. if M_rem > 0 else 0.)
-
-        prediction_ns = np.mean(prediction_nss)
-        prediction_em = np.mean(prediction_ems)
-
-    else:
-        M_rem = computeDiskMass.computeDiskMass(mass_1, mass_2, a_1, a_2)
-        prediction_ns = np.sum(mass_2 <= threshold)/len(mass_2)
-        prediction_em = np.sum(M_rem > 0)/len(M_rem)
-
-    prediction_mg = (mass_1 <= 5) & (mass_1 >= 3)
-    prediction_mg += (mass_2 <= 5) & (mass_2 >= 3)
-    prediction_mg = np.sum(prediction_mg)/len(mass_1)
-
-    return prediction_ns, prediction_em, prediction_mg
+"""Module containing tools for EM-Bright classification of
+compact binaries using trained supervised classifier
+"""
+import h5py
+import numpy as np
+from scipy.interpolate import interp1d
+from astropy import cosmology, units as u
+
+from . import computeDiskMass, utils
+from .data import EOS_BAYES_FACTORS, PACKAGE_FILENAMES
+
+ALL_EOS_DRAWS = utils.load_eos_posterior()
+
+_classifiers = {
+    eos: utils._open_and_return_clfs(
+        PACKAGE_FILENAMES[f'{eos}.pickle']
+    )
+    for eos in EOS_BAYES_FACTORS
+}
+"""Classifiers keyed on EOS names. Order (clf_ns, clf_em)"""
+assert set(_classifiers) == set(EOS_BAYES_FACTORS), "Inconsistency in"
+" number of trained classifiers."
+
+_massgap_classifier = utils._open_and_return_clfs(
+        PACKAGE_FILENAMES['MASS_GAP.pickle']
+    )
+
+
+def mchirp(mass_1, mass_2):
+    return (mass_1 * mass_2)**(3./5.)/(mass_1 + mass_2)**(1./5.)
+
+
+def q(mass_1, mass_2):
+    return mass_2/mass_1 if mass_2 < mass_1 else mass_1/mass_2
+
+
+def source_classification(mass_1, mass_2, chi1, chi2, snr,
+                          ns_classifier=None,
+                          emb_classifier=None,
+                          massgap_classifier=None):
+    """
+    Computes ``HasNS``, ``HasRemnant``, and ``MassGap``
+    probabilities from point mass, spin and
+    signal to noise ratio estimates.
+
+    Parameters
+    ----------
+    mass_1 : float
+        primary mass
+    mass_2 : float
+        secondary mass
+    chi1 : float
+        dimensionless primary spin
+    chi2 : float
+        dimensionless secondary spin
+    snr : float
+        signal to noise ratio of the signal
+    ns_classifier : object, optional
+        pickled object for NS classification
+    emb_classifier : object, optional
+        pickled object for EM brightness classification
+    massgap_classifier : object, optional
+        pickled object for EM brightness classification
+
+    Returns
+    -------
+    tuple
+        (HasNS, HasRemnant, HasMassGap) predicted values.
+    Notes
+    -----
+    By default the classifiers, trained based
+    on different nuclear equations of state (EoSs)
+    are downloaded from the project page:
+    https://git.ligo.org/emfollow/em-properties/em-bright.
+    The methodology is described in arXiv:1911.00116.
+    The score from each classifier is weighted based on
+    the bayes factors of individual EoSs as mentioned in
+    Table I of arXiv:2104.08681.
+    However, if the trained classifiers are supplied
+    via ``ns_classifier`` and ``emb_classifier``,
+    the score is reported based on the classifier instead
+    of re-weighting the score.
+    Examples
+    --------
+    >>> from ligo.em_bright import em_bright
+    >>> em_bright.source_classification(2.0 ,1.0 ,0. ,0. ,10.0)
+    (1.0, 1.0, 0.0)
+    """
+    features = [[mass_1, mass_2, chi1, chi2, snr]]
+    try:
+        # custom classifiers supplied
+        return (
+            ns_classifier.predict_proba(features).T[1][0],
+            emb_classifier.predict_proba(features).T[1][0],
+            massgap_classifier.predict_proba(features).T[1][0]
+        )
+    except AttributeError as e:
+        msg, *_ = e.args
+        if msg != """'NoneType' object has no attribute 'predict_proba'""":
+            raise
+
+    reweighted_ns_score = reweighted_emb_score = 0.
+    for eosname, bayes_factor in EOS_BAYES_FACTORS.items():
+        ns_classifier, emb_classifier = _classifiers[eosname]
+        reweighted_ns_score += ns_classifier.predict_proba(
+            features).T[1][0] * bayes_factor
+        reweighted_emb_score += emb_classifier.predict_proba(
+            features).T[1][0] * bayes_factor
+    massgap_score = _massgap_classifier.predict_proba(features).T[1][0]
+    return reweighted_ns_score, reweighted_emb_score, massgap_score
+
+
+def get_redshifts(distances, N=10000):
+    """
+    Compute redshift using the Planck15 cosmology.
+
+    Parameters
+    ----------
+    distances: float or numpy.ndarray
+              distance(s) in Mpc
+
+    N : int, optional
+      Number of steps for the computation of the interpolation function
+
+    Example
+    -------
+    >>> distances = np.linspace(10, 100, 10)
+    >>> em_bright.get_redshifts(distances)
+    array([0.00225566, 0.00450357, 0.00674384, 0.00897655,
+           0.01120181, 0.0134197 , 0.01563032, 0.01783375
+           0.02003009, 0.02221941])
+
+    Notes
+    -----
+    This function accepts HDF5 posterior samples file and computes
+    redshift by interpolating the distance-redshift relation.
+    """
+    function = cosmology.Planck15.luminosity_distance
+    min_dist = np.min(distances)
+    max_dist = np.max(distances)
+    z_min = cosmology.z_at_value(func=function, fval=min_dist*u.Mpc)
+    z_max = cosmology.z_at_value(func=function, fval=max_dist*u.Mpc)
+    z_steps = np.linspace(z_min - (0.1*z_min), z_max + (0.1*z_max), N)
+    lum_dists = cosmology.Planck15.luminosity_distance(z_steps)
+    s = interp1d(lum_dists, z_steps)
+    redshifts = s(distances)
+    return redshifts
+
+
+def source_classification_pe(posterior_samples_file, threshold=3.0,
+                             num_eos_draws=10000, eos_seed=None,
+                             eosname=None):
+    """
+    Compute ``HasNS``, ``HasRemnant``, and ``HasMassGap`` probabilities
+    from posterior samples.
+
+    Parameters
+    ----------
+    posterior_samples_file : str
+        Posterior samples file
+
+    threshold : float, optional
+        Maximum neutron star mass for `HasNS` computation
+
+    num_eos_draws : int
+        providing an int here runs eos marginalization
+        with the value determining how many eos's to draw
+
+    eos_seed : int
+        seed for random eos draws
+
+    eosname : str
+        Equation of state name, inferred from ``lalsimulation``. Supersedes
+        eos marginalization method when provided.
+
+    Returns
+    -------
+    tuple
+        (HasNS, HasRemnant, HasMassGap) predicted values.
+
+
+    Examples
+    --------
+    >>> from ligo.em_bright import em_bright
+    >>> em_bright.source_classification_pe('posterior_samples.hdf5')
+    (1.0, 0.96, 0.0)
+    """
+    with h5py.File(posterior_samples_file, 'r') as data:
+        samples = data['posterior_samples'][()]
+
+    try:
+        mass_1, mass_2 = samples['mass_1_source'], samples['mass_2_source']
+    except ValueError:
+        lum_dist = samples['luminosity_distance']
+        redshifts = get_redshifts(lum_dist)
+        try:
+            mass_1, mass_2 = samples['mass_1'], samples['mass_2']
+            mass_1, mass_2 = mass_1/(1 + redshifts), mass_2/(1 + redshifts)
+        except ValueError:
+            chirp_mass, mass_ratio = samples['chirp_mass'], samples['mass_ratio']  # noqa:E501
+            chirp_mass = chirp_mass/(1 + redshifts)
+            mass_1 = chirp_mass * (1 + mass_ratio)**(1/5) * (mass_ratio)**(-3/5)  # noqa:E501
+            mass_2 = chirp_mass * (1 + mass_ratio)**(1/5) * (mass_ratio)**(2/5)
+
+    try:
+        a_1 = samples["spin_1z"]
+        a_2 = samples["spin_2z"]
+    except ValueError:
+        try:
+            a_1 = samples['a_1'] * np.cos(samples['tilt_1'])
+            a_2 = samples['a_2'] * np.cos(samples['tilt_2'])
+        except ValueError:
+            a_1, a_2 = np.zeros(len(mass_1)), np.zeros(len(mass_2))
+
+    if eosname:
+        M_rem = computeDiskMass.computeDiskMass(mass_1, mass_2, a_1, a_2,
+                                                eosname=eosname)
+        prediction_ns = np.sum(mass_2 <= threshold)/len(mass_2)
+        prediction_em = np.sum(M_rem > 0)/len(M_rem)
+
+    else:
+        np.random.seed(eos_seed)
+        prediction_nss, prediction_ems = [], []
+        # EoS draws from: 10.5281/zenodo.6502467
+        rand_subset = np.random.choice(
+            len(ALL_EOS_DRAWS), num_eos_draws if num_eos_draws < len(ALL_EOS_DRAWS) else len(ALL_EOS_DRAWS), replace=False)  # noqa:E501
+        subset_draws = ALL_EOS_DRAWS[rand_subset]
+        # convert radius to m from km
+        M, R = subset_draws['M'], 1000*subset_draws['R']
+        max_masses = np.max(M, axis=1)
+        f_M = [interp1d(m, r, bounds_error=False) for m, r in zip(M, R)]
+        for mass_radius_relation, max_mass in zip(f_M, max_masses):
+            M_rem = computeDiskMass.computeDiskMass(mass_1, mass_2, a_1, a_2, eosname=mass_radius_relation, max_mass=max_mass)  # noqa:E501
+            prediction_nss.append(np.mean(mass_2 <= max_mass))
+            prediction_ems.append(np.mean(M_rem > 0))
+
+        prediction_ns = np.mean(prediction_nss)
+        prediction_em = np.mean(prediction_ems)
+
+    prediction_mg = (mass_1 <= 5) & (mass_1 >= 3)
+    prediction_mg += (mass_2 <= 5) & (mass_2 >= 3)
+    prediction_mg = np.sum(prediction_mg)/len(mass_1)
+
+    return prediction_ns, prediction_em, prediction_mg
```

### Comparing `ligo_em_bright-1.1.3/ligo/em_bright/utils.py` & `ligo_em_bright-1.1.4/ligo/em_bright/utils.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,663 +1,663 @@
-# Copyright (C) 2018-2021 Shaon Ghosh, Shasvath Kapadia, Deep Chatterjee
-# 2021-2022 Andrew Toivonen
-#
-# This program is free software; you can redistribute it and/or modify it
-# under the terms of the GNU General Public License as published by the
-# Free Software Foundation; either version 2 of the License, or (at your
-# option) any later version.
-#
-# This program is distributed in the hope that it will be useful, but
-# WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU General
-# Public License for more details.
-#
-# You should have received a copy of the GNU General Public License along
-# with this program; if not, write to the Free Software Foundation, Inc.,
-# 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA.
-
-
-import os
-import pickle
-import re
-
-import h5py
-from argparse import ArgumentParser
-from configparser import ConfigParser
-import glob
-import sqlite3
-
-import numpy as np
-import pandas as pd
-from astropy.table import Column, Table, vstack
-from sklearn.model_selection import KFold
-from sklearn.neighbors import KNeighborsClassifier
-from sklearn.ensemble import RandomForestClassifier
-
-from . import computeDiskMass
-from .data import PACKAGE_FILENAMES, EOS_BAYES_FACTORS, EOS_MAX_MASS
-
-
-def join():
-    """
-    Joins the extracted sim-coinc data from GstLAL injection
-    campaigns into a single Astropy table
-    """
-    parser = ArgumentParser(
-        "Join extracted GstLAL sim-coinc parameters as astropy table")
-    parser.add_argument("-i", "--input", required=True,
-                        help="Directory storing extracted sim-coinc files")
-    parser.add_argument("-c", "--config", required=True,
-                        help="Name of the config file")
-    parser.add_argument("-o", "--output", required=True,
-                        help="Name of the output file")
-    args = parser.parse_args()
-
-    config = ConfigParser()
-    config.read(args.config)
-    extract_prefix = config.get('output_filenames',
-                                'em_bright_extract_prefix')
-    extract_suffix = config.get('output_filenames',
-                                'em_bright_extract_suffix')
-    cols = config.get('core',
-                      'sqlite_cols')
-    list_of_files = glob.glob(
-        os.path.join(args.input, '{}*{}'.format(extract_prefix,
-                                                extract_suffix)))
-    cols = cols.split(',')
-    # FIXME delimited '|' is a fragile piece
-    data = vstack(
-        [Table.read(f, format='ascii', delimiter='|', names=cols)
-         for f in list_of_files]
-    )
-    # FIXME need a better implementation
-    # convert injected detector frame mass to source frame masses
-    inj_mass1_source = Column(data['inj_m1']/(1.0 + data['inj_redshift']),
-                              name='inj_mass1_source_frame')
-    inj_mass2_source = Column(data['inj_m2']/(1.0 + data['inj_redshift']),
-                              name='inj_mass2_source_frame')
-    ID = Column(np.arange(len(data)), name='id')
-    data.add_column(ID, index=0)
-    data.add_column(inj_mass1_source, index=0)
-    data.add_column(inj_mass2_source, index=0)
-
-    data.write(args.output, format='ascii', delimiter='\t')
-
-
-def extract():
-    """
-    Ingests a GstLAL injection campaign sqlite database and
-    outputs the list of coinc parameters in a flat file
-    """
-    parser = ArgumentParser(
-        "Get sim-coinc maps for LIGO GstLAL injection sqlite database")
-    parser.add_argument("-i", "--input", required=True,
-                        help="sqlite database")
-    parser.add_argument("-o", "--output", required=True,
-                        help="Output file, stored as numpy array")
-    args = parser.parse_args()
-
-    cur = sqlite3.connect(args.input).cursor()
-    cur.execute(
-        """
-        CREATE TEMPORARY TABLE
-        sim_coinc_map_helper
-        AS
-        SELECT a.event_id as sid,
-        coinc_event.coinc_event_id as cid,
-        coinc_event.likelihood as lr
-        FROM coinc_event_map as a
-        JOIN coinc_event_map AS b ON (b.coinc_event_id == a.coinc_event_id)
-        JOIN coinc_event ON (coinc_event.coinc_event_id == b.event_id)
-        WHERE a.table_name == 'sim_inspiral'
-        AND b.table_name == 'coinc_event'
-        AND NOT EXISTS (
-            SELECT * FROM time_slide WHERE
-            time_slide.time_slide_id == coinc_event.time_slide_id
-            AND time_slide.offset != 0
-        )"""
-    )
-
-    cur.execute(
-        """
-        CREATE INDEX IF NOT EXISTS
-        sim_coinc_map_helper_index ON sim_coinc_map_helper (sid, cid)
-        """
-    )
-
-    cur.execute(
-        """
-        CREATE TEMPORARY TABLE
-            sim_coinc_map
-        AS
-            SELECT
-                sim_inspiral.simulation_id AS simulation_id,
-                (
-                    SELECT cid FROM
-                                sim_coinc_map_helper
-                    WHERE sid = simulation_id
-                    ORDER BY lr DESC
-                    LIMIT 1
-                ) AS coinc_event_id
-            FROM sim_inspiral
-            WHERE coinc_event_id IS NOT NULL
-        """
-    )
-
-    cur.execute("""DROP INDEX sim_coinc_map_helper_index""")
-
-    query = """
-    SELECT
-    sim_inspiral.mass1,
-    sim_inspiral.mass2,
-    sim_inspiral.spin1z,
-    sim_inspiral.spin2z,
-        sim_inspiral.alpha3,
-    sngl_inspiral.mass1,
-    sngl_inspiral.mass2,
-    sngl_inspiral.spin1z,
-    sngl_inspiral.spin2z,
-    sngl_inspiral.Gamma1,
-    coinc_inspiral.combined_far,
-    coinc_inspiral.snr,
-    coinc_inspiral.end_time
-    FROM
-    sim_coinc_map
-    JOIN
-    sim_inspiral
-    ON
-    sim_coinc_map.simulation_id==sim_inspiral.simulation_id
-    JOIN
-    coinc_event_map
-    ON
-    sim_coinc_map.coinc_event_id == coinc_event_map.coinc_event_id
-    JOIN
-    coinc_inspiral
-    ON
-    sim_coinc_map.coinc_event_id == coinc_inspiral.coinc_event_id
-    JOIN
-    sngl_inspiral
-    ON (
-        coinc_event_map.table_name == 'sngl_inspiral'
-        AND coinc_event_map.event_id == sngl_inspiral.event_id
-    )
-    WHERE
-    sngl_inspiral.ifo=='H1';
-    """
-    np.savetxt(args.output, np.array(cur.execute(query).fetchall()),
-               fmt='%f|%f|%f|%f|%f|%f|%f|%f|%f|%d|%e|%f|%f')
-
-
-def train():
-    parser = ArgumentParser(
-        description='Executable to train source classifier from injections')
-
-    parser.add_argument(
-        '-i', '--input',
-        help='Pickled dataframe containing source categorized data')
-    parser.add_argument(
-        '-o', '--output',
-        help='Pickled object storing the trained classifiers')
-    parser.add_argument(
-        '-d', '--param-sweep-plot-prefix', default=None,
-        help='Supply filename prefix to output a parameter sweep plot')
-    parser.add_argument(
-        '-c', '--config', required=True,
-        help='Config file with additional parameters')
-    parser.add_argument("--mass-gap", required=False, action="store_true",
-                        help="mode of categorization")
-
-    args = parser.parse_args()
-    if args.mass_gap:
-        settings = 'massgap'
-    else:
-        settings = 'em_bright'
-    config = ConfigParser()
-    config.read(args.config)
-    # compulsory sections in config
-    required_sections = ['core',
-                         'em_bright']
-    assert all(config.has_section(s) for s in required_sections), \
-        'Config file must have sections %s' % (required_sections,)
-
-    # get column names and values from config
-    feature_cols = config.get(settings,
-                              'feature_cols').split(',')
-    category_cols = config.get(settings,
-                               'category_cols').split(',')
-    threshold_cols = config.get(settings,
-                                'threshold_cols').split(',')
-    all_cols = feature_cols + category_cols + threshold_cols
-
-    threshold_values = map(
-        eval, config.get(
-            settings,
-            'threshold_values').split(',')
-        )
-    threshold_type = config.get(settings,
-                                'threshold_type').split(',')
-    # read dataframe, check sanity
-    with open(args.input, 'rb') as f:
-        df = pickle.load(f)
-
-    assert all(col in df.keys() for col in all_cols), \
-        'Dataframe must contain columns %s' % (all_cols,)
-
-    # create masked array based on threshold values,
-    # extract features and targets
-    mask = np.ones(len(df)).astype(bool)
-    for col, value, typ in zip(threshold_cols, threshold_values,
-                               threshold_type):
-        mask &= df[col] < value if typ == 'lesser' else \
-            df[col] > value if typ == 'greater' else True
-
-    features = df[feature_cols][mask]
-    targets = df[category_cols][mask]
-
-    if not args.mass_gap:
-        clf_kwargs = eval(config.get('em_bright',
-                                     'clf_kwargs'))
-        if clf_kwargs.get('metric') == 'mahalanobis':
-            clf_kwargs['metric_params'] = dict(
-                V=features.cov().values
-            )  # covariance matrix needed for mahalanobis metric
-        clfs = []
-        for category, target_value in targets.iteritems():
-            # run KFold cross-validation
-            res_predict, res_predict_proba = run_k_fold_split(
-                features, target_value,
-                training_task=run_KNN_classifier,
-                **clf_kwargs)
-            test_results = pd.DataFrame(
-                np.vstack((features.T, target_value,
-                           res_predict, res_predict_proba)).T,
-                columns=feature_cols + ['targets', 'predict', 'predict_proba']
-            )
-            test_results_filename = 'cross-val-res-' + category + '.csv'
-            test_results.to_csv(test_results_filename, index=False)
-            # train on the full dataset
-            clf = KNeighborsClassifier(**clf_kwargs)
-            clf.fit(features.values, target_value)
-            if args.param_sweep_plot_prefix:
-                _create_param_sweep_plot(
-                    clf, category,
-                    args.param_sweep_plot_prefix
-                )
-            clfs.append(clf)
-        # append the output filename of the classifier
-        clfs.extend([args.output])
-        with open(args.output, 'wb') as f:
-            pickle.dump(clfs, f)
-    else:
-        # train random forest classifier for massgap category
-        clf_kwargs = eval(config.get('massgap',
-                                     'clf_kwargs'))
-        res_predict, res_predict_proba = run_k_fold_split(
-            features, targets,
-            training_task=run_RF_classifier, **clf_kwargs
-        )
-        test_results = pd.DataFrame(
-            np.vstack((features.T, targets.squeeze().T,
-                       res_predict, res_predict_proba)).T,
-            columns=feature_cols + ['targets', 'predict', 'predict_proba']
-        )
-        test_results_filename = 'cross-val-res-' + 'mass-gap' + '.csv'
-        test_results.to_csv(test_results_filename, index=False)
-        clf = RandomForestClassifier(**clf_kwargs)
-        clf.fit(features.values, targets.squeeze())
-        _create_param_sweep_plot(
-            clf, 'mass_gap',
-            prefix='SLy'  # FIXME: ad-hoc prefix needed, not used for plotting
-        )
-        with open(args.output, 'wb') as f:
-            # append the filename of the classfier
-            pickle.dump([clf, args.output], f)
-
-
-def _open_and_return_clfs(filename):
-    """Unpack pickle files storing classifier and return.
-    If two classifiers exist, assume first argument is HasNS,
-    second HasRemnant. If single classifier exists, then assume
-    mass_gap classifier.
-    """
-    with open(filename, 'rb') as f:
-        content = pickle.load(f)
-        try:
-            clf_ns, clf_em, _filename = content
-            return clf_ns, clf_em
-        except ValueError:
-            clf_mass_gap, _filename = content
-            return clf_mass_gap
-
-
-def _get_mass_grid():
-    """Get a grid over mass1, mass2. Used for parameter sweep."""
-    mass1 = np.linspace(1, 20, 200)
-    mass2 = np.linspace(1, 20, 200)
-    t = Table(
-        data=np.vstack(
-            (np.repeat(mass1, mass2.size),
-             np.tile(mass2, mass1.size))
-        ).T, names=('mass1', 'mass2')
-    )
-    mask = t['mass1'] > t['mass2']
-    t = t[mask]
-    return t
-
-
-def _get_param_sweep(clf):
-    """Create a fake recovered parameter space return
-    the predictions for the classifier sweeping across
-    masses.
-    """
-    if hasattr(clf, 'metric') and clf.metric == "mahalanobis":
-        clf.n_jobs = 1  # issue with BallTree output
-    t = _get_mass_grid()
-    spins = Table(
-        data=np.vstack(
-            (np.repeat(np.linspace(0, 1, 2), 2),
-             np.tile(np.linspace(0, 1, 2), 2))
-        ).T,
-        names=('chi1', 'chi2')
-    )
-    SNR = 10.
-    res = list()
-    for spin_vals in spins:
-        SNR *= np.ones(len(t))
-        chi1 = spin_vals['chi1'] * np.ones(len(t))
-        chi2 = spin_vals['chi2'] * np.ones(len(t))
-        # make predictions and make plots
-        param_sweep_features = np.stack(
-            [t['mass1'], t['mass2'], chi1, chi2, SNR]
-        ).T
-        predictions = clf.predict_proba(param_sweep_features).T[1]
-        res.append((param_sweep_features, predictions))
-    return res
-
-
-def _create_param_sweep_plot(clf, category, prefix=None):
-    """Create a parameter sweep plot using the supplied classifer"""
-    import matplotlib.pyplot as plt
-    res = _get_param_sweep(clf)
-    fig = plt.figure(figsize=(14, 20))
-    for idx, r in enumerate(res):
-        features, predictions = r
-        # FIXME: Ugly, but works
-        title = "chi1 = {0}; chi2 = {1}; SNR = {2}".format(
-            features[0][2], features[0][3],
-            features[0][4]
-        )
-        make_plots(
-            features, predictions, title,
-            (fig, idx+1), prefix=prefix, category=category
-        )
-    try:
-        plt.savefig(prefix+'_param_sweep_'+category+'.png')
-    except TypeError:
-        plt.savefig('param_sweep_'+category+'.png')
-
-
-def load_eos_posterior():
-    '''
-    Loads eos posterior draws (https://zenodo.org/record/6502467#.Yoa2EKjMI2z)
-
-    Returns
-    -------
-    draws: np.array
-        equally weighted eos draws from file
-    '''
-    eos_file = PACKAGE_FILENAMES['EOS_POSTERIOR_DRAWS.h5']
-    with h5py.File(eos_file, 'r') as f:
-        draws = np.array(f['EOS'])
-    return draws
-
-
-def param_sweep_plot():
-    """Create parameter sweep plot, weighting classifier
-    results using bayes factor
-    """
-    parser = ArgumentParser(
-        "Create a parameter sweep, EoS predictions based")
-    parser.add_argument("-i", "--input", required=True,
-                        help="Directory storing trained classifier files")
-    parser.add_argument("-c", "--config", required=True,
-                        help="Config file")
-    parser.add_argument("-v", "--verbose", action='store_true',
-                        help="show progress")
-    args = parser.parse_args()
-
-    config = ConfigParser()
-    config.read(args.config)
-
-    train_prefix = config.get('output_filenames', 'em_bright_train_prefix')
-    train_suffix = config.get('output_filenames', 'em_bright_train_suffix')
-    clf_filenames = glob.glob(
-        os.path.join(args.input, f'{train_prefix}*{train_suffix}'))
-    if args.verbose:
-        print("Trained classifers", clf_filenames)
-    assert clf_filenames, "No files found. Check directory."
-    reweight_ns = dict.fromkeys(EOS_BAYES_FACTORS)
-    reweight_em = dict.fromkeys(EOS_BAYES_FACTORS)
-    import matplotlib.pyplot as plt
-    for fname in clf_filenames:
-        if args.verbose:
-            print(fname)
-        clf_ns, clf_em = _open_and_return_clfs(fname)
-        eosname, *_ = filter(
-            lambda _: re.match(
-                ".*" + _ + config.get('output_filenames',
-                                      'em_bright_train_suffix'),
-                fname
-            ), EOS_BAYES_FACTORS
-        )
-        res_ns = _get_param_sweep(clf_ns)
-        res_em = _get_param_sweep(clf_em)
-        reweight_ns.update(
-            {
-                eosname: dict(
-                    features=np.array(
-                        [f for f, p in res_ns]
-                    ),
-                    predictions=np.array(
-                        [p * EOS_BAYES_FACTORS[eosname] for f, p in res_ns]
-                    )
-                )
-            }
-        )
-        reweight_em.update(
-            {
-                eosname: dict(
-                    features=np.array(
-                        [f for f, p in res_em]
-                    ),
-                    predictions=np.array(
-                        [p * EOS_BAYES_FACTORS[eosname] for f, p in res_em]
-                    )
-                )
-            }
-        )
-    assert all(reweight_ns.values()), "Missing some listed EOSs."
-    assert all(reweight_em.values()), "Missing some listed EOSs."
-    reweighted_score_ns = np.sum(
-        [v['predictions'] for v in reweight_ns.values()],
-        axis=0
-    )
-    reweighted_score_em = np.sum(
-        [v['predictions'] for v in reweight_em.values()],
-        axis=0
-    )
-    for category, score in zip(
-            ["NS", "EMB"], [reweighted_score_ns, reweighted_score_em]):
-        fig = plt.figure(figsize=(14, 20))
-        for idx, (f, p) in enumerate(
-                zip(reweight_ns['SLy']['features'], score)):
-            title = "chi1 = {0}; chi2 = {1}; SNR = {2}".format(
-                f[0][2], f[0][3], f[0][4])
-            make_plots(
-                f, p, title, (fig, idx+1),
-                prefix='SLy', category=category
-            )
-        plt.savefig("reweighted_" + category + "_param_sweep.png")
-
-
-def make_plots(features, predictions, title, fig_idx,
-               prefix=None, category=None):
-    import matplotlib.pyplot as plt
-    fig_, idx = fig_idx
-    fig_.add_subplot(4, 1, idx)
-    # indices 0 and 1 correspond to mass1 and mass2 respectively
-    plt.scatter(features.T[0], features.T[1],
-                s=10, c=predictions)
-    plt.title(title)
-    plt.tight_layout()
-    plt.colorbar(label='Probability')
-    # plot chirp mass contours
-    m1 = np.linspace(1, 20, 1000)
-    m2 = np.linspace(1, 20, 1000)
-    M1, M2 = np.meshgrid(m1, m2)
-    s1z = np.unique(features.T[2])[0]*np.ones(M1.shape)
-    s2z = np.unique(features.T[3])[0]*np.ones(M2.shape)
-    rem_masses = list()
-    for _ in range(M1.shape[0]):
-        rem_masses.append(
-            computeDiskMass.computeDiskMass(
-                M1[_], M2[_], s1z[_], s2z[_],
-                eosname=prefix
-            )
-        )
-    rem_masses = np.array(rem_masses).reshape(M1.shape)
-    Mc = (M1*M2)**(3./5.)/(M1 + M2)**(1./5.)
-    mask = M1 > M2
-    M1 = np.ma.masked_array(M1, mask=mask)
-    M2 = np.ma.masked_array(M2, mask=mask)
-    s1z = np.ma.masked_array(s1z, mask=mask)
-    s2z = np.ma.masked_array(s2z, mask=mask)
-    Mc = np.ma.masked_array(Mc, mask=mask)
-    rem_masses = np.ma.masked_array(
-        rem_masses, mask=mask*(M2 > EOS_MAX_MASS[prefix])
-    )
-    CS = plt.contour(
-        M1, M2, Mc.T, levels=[2.01, 2.22, 2.99, 3.48, 4.73, 5.4],
-        # (m1, m2) = (4, 1.4) -> Mc = 2.01
-        # (m1, m2) = (5, 1.4) -> Mc = 2.22
-        # (m1, m2) = (10, 1.4) -> Mc = 2.99
-        # (m1, m2) = (4, 4)    -> Mc = 3.48
-        # (m1, m2) = (30, 1.4) -> Mc = 4.73
-        # (m1, m2) = (10, 4)  -> Mc = 5.4
-        # three different NSBH populations;
-        # three different mass-gap populations
-        colors='black', linewidths=1.0
-    )
-    plt.clabel(CS, inline=True, fontsize=16)
-    plt.xlim((1, 20))
-    plt.ylim((1, 12))
-    try:
-        max_mass = EOS_MAX_MASS[prefix]
-    except KeyError:
-        max_mass = 3.0
-    if 'NS' in category:
-        plt.axhline(y=max_mass, c='r', linewidth=1.2)
-    elif 'EM' in category:
-        CS = plt.contour(M1, M2, rem_masses.T,
-                         levels=[0., ], colors='red',
-                         linewidths=1.2)
-    plt.xlabel(r'$m_1$', fontsize=16)
-    plt.ylabel(r'$m_2$', fontsize=16)
-
-
-def run_k_fold_split(features, targets, n_splits=10, random_state=0,
-                     training_task=None, **kwargs):
-    """Split the `features` in `n_splits`, train on `n_splits - 1`
-    sets, test on the last fraction. This performed across the complete
-    dataset.
-
-    Parameters
-    ----------
-    features : numpy.ndarray
-        Feature set
-    targets : numpy.ndarray
-        Target set containing binary classification of `features`
-    n_splits : int
-        Number of splits for `features` and `targets`
-    random_state : int
-        Random seed for the split
-    training_task : callable
-        function with arguments (X_train, y_train, X_test, **kwargs) which
-        trains, and returns predictions on X_test.
-        E.g. :meth:`run_KNN_classifier`,
-        or :meth:`run_RF_classifier`.
-    **kwargs
-        Keyword arguments passed to `training_task`.
-
-    Returns
-    -------
-    tuple
-        (res_predict, res_predict_proba) - predictions and probabilities
-    """
-    res_predict_proba = np.empty(len(features))
-    res_predict = np.empty(len(features))
-    res_predict_proba[:] = np.nan
-    res_predict[:] = np.nan
-
-    sss = KFold(n_splits=n_splits, shuffle=True, random_state=random_state)
-    sss.get_n_splits(features, targets)
-    for train_index, test_index in sss.split(features, targets):
-        X_train, X_test, y_train = \
-            features.iloc[train_index], \
-            features.iloc[test_index], \
-            targets.iloc[train_index]
-
-        predict_proba, predict = training_task(X_train, y_train, X_test,
-                                               **kwargs)
-        # second column is the prob of NS/EMB
-        predict_proba = predict_proba.T[1]
-
-        res_predict_proba[test_index] = predict_proba
-        res_predict[test_index] = predict
-    return res_predict, res_predict_proba
-
-
-def run_KNN_classifier(X_train, y_train,
-                       X_test,
-                       **kwargs):
-    '''
-    Run KNearestNeighborClassifier classifier returns
-    `clf.predict_proba`
-
-    Parameters
-    ----------
-    X_train : numpy.ndarray
-        Feature training set, can be array or Dataframe
-    y_train : numpy.array
-        Target training set, 0 or 1 binary classification
-    X_test : numpy.ndarray
-        Feature testing set, can be array or DataFrame
-    '''
-    if kwargs.get('metric') == 'mahalanobis':
-        kwargs['n_jobs'] = 1  # issue with KDTree, BallTree with n_jobs > 1
-    clf = KNeighborsClassifier(**kwargs)
-    clf.fit(X_train.values, y_train)
-    predictions_proba = clf.predict_proba(X_test)
-    predict = clf.predict(X_test)
-    return predictions_proba, predict
-
-
-def run_RF_classifier(X_train, y_train, X_test,
-                      **kwargs):
-    '''
-    Run RandomForestClassifier; returns
-    `clf.predict_proba`
-
-    Parameters
-    ----------
-    X_train : numpy.ndarray
-        Feature training set, can be array or Dataframe
-    y_train : numpy.array
-        Target training set, 0 or 1 binary classification
-    X_test : numpy.ndarray
-        Feature testing set, can be array or DataFrame
-    '''
-    clf = RandomForestClassifier(**kwargs)
-    clf.fit(X_train.values, y_train)
-    predictions_proba = clf.predict_proba(X_test)
-    predict = clf.predict(X_test)
-    return predictions_proba, predict
+# Copyright (C) 2018-2021 Shaon Ghosh, Shasvath Kapadia, Deep Chatterjee
+# 2021-2022 Andrew Toivonen
+#
+# This program is free software; you can redistribute it and/or modify it
+# under the terms of the GNU General Public License as published by the
+# Free Software Foundation; either version 2 of the License, or (at your
+# option) any later version.
+#
+# This program is distributed in the hope that it will be useful, but
+# WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU General
+# Public License for more details.
+#
+# You should have received a copy of the GNU General Public License along
+# with this program; if not, write to the Free Software Foundation, Inc.,
+# 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA.
+
+
+import os
+import pickle
+import re
+
+import h5py
+from argparse import ArgumentParser
+from configparser import ConfigParser
+import glob
+import sqlite3
+
+import numpy as np
+import pandas as pd
+from astropy.table import Column, Table, vstack
+from sklearn.model_selection import KFold
+from sklearn.neighbors import KNeighborsClassifier
+from sklearn.ensemble import RandomForestClassifier
+
+from . import computeDiskMass
+from .data import PACKAGE_FILENAMES, EOS_BAYES_FACTORS, EOS_MAX_MASS
+
+
+def join():
+    """
+    Joins the extracted sim-coinc data from GstLAL injection
+    campaigns into a single Astropy table
+    """
+    parser = ArgumentParser(
+        "Join extracted GstLAL sim-coinc parameters as astropy table")
+    parser.add_argument("-i", "--input", required=True,
+                        help="Directory storing extracted sim-coinc files")
+    parser.add_argument("-c", "--config", required=True,
+                        help="Name of the config file")
+    parser.add_argument("-o", "--output", required=True,
+                        help="Name of the output file")
+    args = parser.parse_args()
+
+    config = ConfigParser()
+    config.read(args.config)
+    extract_prefix = config.get('output_filenames',
+                                'em_bright_extract_prefix')
+    extract_suffix = config.get('output_filenames',
+                                'em_bright_extract_suffix')
+    cols = config.get('core',
+                      'sqlite_cols')
+    list_of_files = glob.glob(
+        os.path.join(args.input, '{}*{}'.format(extract_prefix,
+                                                extract_suffix)))
+    cols = cols.split(',')
+    # FIXME delimited '|' is a fragile piece
+    data = vstack(
+        [Table.read(f, format='ascii', delimiter='|', names=cols)
+         for f in list_of_files]
+    )
+    # FIXME need a better implementation
+    # convert injected detector frame mass to source frame masses
+    inj_mass1_source = Column(data['inj_m1']/(1.0 + data['inj_redshift']),
+                              name='inj_mass1_source_frame')
+    inj_mass2_source = Column(data['inj_m2']/(1.0 + data['inj_redshift']),
+                              name='inj_mass2_source_frame')
+    ID = Column(np.arange(len(data)), name='id')
+    data.add_column(ID, index=0)
+    data.add_column(inj_mass1_source, index=0)
+    data.add_column(inj_mass2_source, index=0)
+
+    data.write(args.output, format='ascii', delimiter='\t')
+
+
+def extract():
+    """
+    Ingests a GstLAL injection campaign sqlite database and
+    outputs the list of coinc parameters in a flat file
+    """
+    parser = ArgumentParser(
+        "Get sim-coinc maps for LIGO GstLAL injection sqlite database")
+    parser.add_argument("-i", "--input", required=True,
+                        help="sqlite database")
+    parser.add_argument("-o", "--output", required=True,
+                        help="Output file, stored as numpy array")
+    args = parser.parse_args()
+
+    cur = sqlite3.connect(args.input).cursor()
+    cur.execute(
+        """
+        CREATE TEMPORARY TABLE
+        sim_coinc_map_helper
+        AS
+        SELECT a.event_id as sid,
+        coinc_event.coinc_event_id as cid,
+        coinc_event.likelihood as lr
+        FROM coinc_event_map as a
+        JOIN coinc_event_map AS b ON (b.coinc_event_id == a.coinc_event_id)
+        JOIN coinc_event ON (coinc_event.coinc_event_id == b.event_id)
+        WHERE a.table_name == 'sim_inspiral'
+        AND b.table_name == 'coinc_event'
+        AND NOT EXISTS (
+            SELECT * FROM time_slide WHERE
+            time_slide.time_slide_id == coinc_event.time_slide_id
+            AND time_slide.offset != 0
+        )"""
+    )
+
+    cur.execute(
+        """
+        CREATE INDEX IF NOT EXISTS
+        sim_coinc_map_helper_index ON sim_coinc_map_helper (sid, cid)
+        """
+    )
+
+    cur.execute(
+        """
+        CREATE TEMPORARY TABLE
+            sim_coinc_map
+        AS
+            SELECT
+                sim_inspiral.simulation_id AS simulation_id,
+                (
+                    SELECT cid FROM
+                                sim_coinc_map_helper
+                    WHERE sid = simulation_id
+                    ORDER BY lr DESC
+                    LIMIT 1
+                ) AS coinc_event_id
+            FROM sim_inspiral
+            WHERE coinc_event_id IS NOT NULL
+        """
+    )
+
+    cur.execute("""DROP INDEX sim_coinc_map_helper_index""")
+
+    query = """
+    SELECT
+    sim_inspiral.mass1,
+    sim_inspiral.mass2,
+    sim_inspiral.spin1z,
+    sim_inspiral.spin2z,
+        sim_inspiral.alpha3,
+    sngl_inspiral.mass1,
+    sngl_inspiral.mass2,
+    sngl_inspiral.spin1z,
+    sngl_inspiral.spin2z,
+    sngl_inspiral.Gamma1,
+    coinc_inspiral.combined_far,
+    coinc_inspiral.snr,
+    coinc_inspiral.end_time
+    FROM
+    sim_coinc_map
+    JOIN
+    sim_inspiral
+    ON
+    sim_coinc_map.simulation_id==sim_inspiral.simulation_id
+    JOIN
+    coinc_event_map
+    ON
+    sim_coinc_map.coinc_event_id == coinc_event_map.coinc_event_id
+    JOIN
+    coinc_inspiral
+    ON
+    sim_coinc_map.coinc_event_id == coinc_inspiral.coinc_event_id
+    JOIN
+    sngl_inspiral
+    ON (
+        coinc_event_map.table_name == 'sngl_inspiral'
+        AND coinc_event_map.event_id == sngl_inspiral.event_id
+    )
+    WHERE
+    sngl_inspiral.ifo=='H1';
+    """
+    np.savetxt(args.output, np.array(cur.execute(query).fetchall()),
+               fmt='%f|%f|%f|%f|%f|%f|%f|%f|%f|%d|%e|%f|%f')
+
+
+def train():
+    parser = ArgumentParser(
+        description='Executable to train source classifier from injections')
+
+    parser.add_argument(
+        '-i', '--input',
+        help='Pickled dataframe containing source categorized data')
+    parser.add_argument(
+        '-o', '--output',
+        help='Pickled object storing the trained classifiers')
+    parser.add_argument(
+        '-d', '--param-sweep-plot-prefix', default=None,
+        help='Supply filename prefix to output a parameter sweep plot')
+    parser.add_argument(
+        '-c', '--config', required=True,
+        help='Config file with additional parameters')
+    parser.add_argument("--mass-gap", required=False, action="store_true",
+                        help="mode of categorization")
+
+    args = parser.parse_args()
+    if args.mass_gap:
+        settings = 'massgap'
+    else:
+        settings = 'em_bright'
+    config = ConfigParser()
+    config.read(args.config)
+    # compulsory sections in config
+    required_sections = ['core',
+                         'em_bright']
+    assert all(config.has_section(s) for s in required_sections), \
+        'Config file must have sections %s' % (required_sections,)
+
+    # get column names and values from config
+    feature_cols = config.get(settings,
+                              'feature_cols').split(',')
+    category_cols = config.get(settings,
+                               'category_cols').split(',')
+    threshold_cols = config.get(settings,
+                                'threshold_cols').split(',')
+    all_cols = feature_cols + category_cols + threshold_cols
+
+    threshold_values = map(
+        eval, config.get(
+            settings,
+            'threshold_values').split(',')
+        )
+    threshold_type = config.get(settings,
+                                'threshold_type').split(',')
+    # read dataframe, check sanity
+    with open(args.input, 'rb') as f:
+        df = pickle.load(f)
+
+    assert all(col in df.keys() for col in all_cols), \
+        'Dataframe must contain columns %s' % (all_cols,)
+
+    # create masked array based on threshold values,
+    # extract features and targets
+    mask = np.ones(len(df)).astype(bool)
+    for col, value, typ in zip(threshold_cols, threshold_values,
+                               threshold_type):
+        mask &= df[col] < value if typ == 'lesser' else \
+            df[col] > value if typ == 'greater' else True
+
+    features = df[feature_cols][mask]
+    targets = df[category_cols][mask]
+
+    if not args.mass_gap:
+        clf_kwargs = eval(config.get('em_bright',
+                                     'clf_kwargs'))
+        if clf_kwargs.get('metric') == 'mahalanobis':
+            clf_kwargs['metric_params'] = dict(
+                V=features.cov().values
+            )  # covariance matrix needed for mahalanobis metric
+        clfs = []
+        for category, target_value in targets.iteritems():
+            # run KFold cross-validation
+            res_predict, res_predict_proba = run_k_fold_split(
+                features, target_value,
+                training_task=run_KNN_classifier,
+                **clf_kwargs)
+            test_results = pd.DataFrame(
+                np.vstack((features.T, target_value,
+                           res_predict, res_predict_proba)).T,
+                columns=feature_cols + ['targets', 'predict', 'predict_proba']
+            )
+            test_results_filename = 'cross-val-res-' + category + '.csv'
+            test_results.to_csv(test_results_filename, index=False)
+            # train on the full dataset
+            clf = KNeighborsClassifier(**clf_kwargs)
+            clf.fit(features.values, target_value)
+            if args.param_sweep_plot_prefix:
+                _create_param_sweep_plot(
+                    clf, category,
+                    args.param_sweep_plot_prefix
+                )
+            clfs.append(clf)
+        # append the output filename of the classifier
+        clfs.extend([args.output])
+        with open(args.output, 'wb') as f:
+            pickle.dump(clfs, f)
+    else:
+        # train random forest classifier for massgap category
+        clf_kwargs = eval(config.get('massgap',
+                                     'clf_kwargs'))
+        res_predict, res_predict_proba = run_k_fold_split(
+            features, targets,
+            training_task=run_RF_classifier, **clf_kwargs
+        )
+        test_results = pd.DataFrame(
+            np.vstack((features.T, targets.squeeze().T,
+                       res_predict, res_predict_proba)).T,
+            columns=feature_cols + ['targets', 'predict', 'predict_proba']
+        )
+        test_results_filename = 'cross-val-res-' + 'mass-gap' + '.csv'
+        test_results.to_csv(test_results_filename, index=False)
+        clf = RandomForestClassifier(**clf_kwargs)
+        clf.fit(features.values, targets.squeeze())
+        _create_param_sweep_plot(
+            clf, 'mass_gap',
+            prefix='SLy'  # FIXME: ad-hoc prefix needed, not used for plotting
+        )
+        with open(args.output, 'wb') as f:
+            # append the filename of the classfier
+            pickle.dump([clf, args.output], f)
+
+
+def _open_and_return_clfs(filename):
+    """Unpack pickle files storing classifier and return.
+    If two classifiers exist, assume first argument is HasNS,
+    second HasRemnant. If single classifier exists, then assume
+    mass_gap classifier.
+    """
+    with open(filename, 'rb') as f:
+        content = pickle.load(f)
+        try:
+            clf_ns, clf_em, _filename = content
+            return clf_ns, clf_em
+        except ValueError:
+            clf_mass_gap, _filename = content
+            return clf_mass_gap
+
+
+def _get_mass_grid():
+    """Get a grid over mass1, mass2. Used for parameter sweep."""
+    mass1 = np.linspace(1, 20, 200)
+    mass2 = np.linspace(1, 20, 200)
+    t = Table(
+        data=np.vstack(
+            (np.repeat(mass1, mass2.size),
+             np.tile(mass2, mass1.size))
+        ).T, names=('mass1', 'mass2')
+    )
+    mask = t['mass1'] > t['mass2']
+    t = t[mask]
+    return t
+
+
+def _get_param_sweep(clf):
+    """Create a fake recovered parameter space return
+    the predictions for the classifier sweeping across
+    masses.
+    """
+    if hasattr(clf, 'metric') and clf.metric == "mahalanobis":
+        clf.n_jobs = 1  # issue with BallTree output
+    t = _get_mass_grid()
+    spins = Table(
+        data=np.vstack(
+            (np.repeat(np.linspace(0, 1, 2), 2),
+             np.tile(np.linspace(0, 1, 2), 2))
+        ).T,
+        names=('chi1', 'chi2')
+    )
+    SNR = 10.
+    res = list()
+    for spin_vals in spins:
+        SNR *= np.ones(len(t))
+        chi1 = spin_vals['chi1'] * np.ones(len(t))
+        chi2 = spin_vals['chi2'] * np.ones(len(t))
+        # make predictions and make plots
+        param_sweep_features = np.stack(
+            [t['mass1'], t['mass2'], chi1, chi2, SNR]
+        ).T
+        predictions = clf.predict_proba(param_sweep_features).T[1]
+        res.append((param_sweep_features, predictions))
+    return res
+
+
+def _create_param_sweep_plot(clf, category, prefix=None):
+    """Create a parameter sweep plot using the supplied classifer"""
+    import matplotlib.pyplot as plt
+    res = _get_param_sweep(clf)
+    fig = plt.figure(figsize=(14, 20))
+    for idx, r in enumerate(res):
+        features, predictions = r
+        # FIXME: Ugly, but works
+        title = "chi1 = {0}; chi2 = {1}; SNR = {2}".format(
+            features[0][2], features[0][3],
+            features[0][4]
+        )
+        make_plots(
+            features, predictions, title,
+            (fig, idx+1), prefix=prefix, category=category
+        )
+    try:
+        plt.savefig(prefix+'_param_sweep_'+category+'.png')
+    except TypeError:
+        plt.savefig('param_sweep_'+category+'.png')
+
+
+def load_eos_posterior():
+    '''
+    Loads eos posterior draws (https://zenodo.org/record/6502467#.Yoa2EKjMI2z)
+
+    Returns
+    -------
+    draws: np.array
+        equally weighted eos draws from file
+    '''
+    eos_file = PACKAGE_FILENAMES['EOS_POSTERIOR_DRAWS.h5']
+    with h5py.File(eos_file, 'r') as f:
+        draws = np.array(f['EOS'])
+    return draws
+
+
+def param_sweep_plot():
+    """Create parameter sweep plot, weighting classifier
+    results using bayes factor
+    """
+    parser = ArgumentParser(
+        "Create a parameter sweep, EoS predictions based")
+    parser.add_argument("-i", "--input", required=True,
+                        help="Directory storing trained classifier files")
+    parser.add_argument("-c", "--config", required=True,
+                        help="Config file")
+    parser.add_argument("-v", "--verbose", action='store_true',
+                        help="show progress")
+    args = parser.parse_args()
+
+    config = ConfigParser()
+    config.read(args.config)
+
+    train_prefix = config.get('output_filenames', 'em_bright_train_prefix')
+    train_suffix = config.get('output_filenames', 'em_bright_train_suffix')
+    clf_filenames = glob.glob(
+        os.path.join(args.input, f'{train_prefix}*{train_suffix}'))
+    if args.verbose:
+        print("Trained classifers", clf_filenames)
+    assert clf_filenames, "No files found. Check directory."
+    reweight_ns = dict.fromkeys(EOS_BAYES_FACTORS)
+    reweight_em = dict.fromkeys(EOS_BAYES_FACTORS)
+    import matplotlib.pyplot as plt
+    for fname in clf_filenames:
+        if args.verbose:
+            print(fname)
+        clf_ns, clf_em = _open_and_return_clfs(fname)
+        eosname, *_ = filter(
+            lambda _: re.match(
+                ".*" + _ + config.get('output_filenames',
+                                      'em_bright_train_suffix'),
+                fname
+            ), EOS_BAYES_FACTORS
+        )
+        res_ns = _get_param_sweep(clf_ns)
+        res_em = _get_param_sweep(clf_em)
+        reweight_ns.update(
+            {
+                eosname: dict(
+                    features=np.array(
+                        [f for f, p in res_ns]
+                    ),
+                    predictions=np.array(
+                        [p * EOS_BAYES_FACTORS[eosname] for f, p in res_ns]
+                    )
+                )
+            }
+        )
+        reweight_em.update(
+            {
+                eosname: dict(
+                    features=np.array(
+                        [f for f, p in res_em]
+                    ),
+                    predictions=np.array(
+                        [p * EOS_BAYES_FACTORS[eosname] for f, p in res_em]
+                    )
+                )
+            }
+        )
+    assert all(reweight_ns.values()), "Missing some listed EOSs."
+    assert all(reweight_em.values()), "Missing some listed EOSs."
+    reweighted_score_ns = np.sum(
+        [v['predictions'] for v in reweight_ns.values()],
+        axis=0
+    )
+    reweighted_score_em = np.sum(
+        [v['predictions'] for v in reweight_em.values()],
+        axis=0
+    )
+    for category, score in zip(
+            ["NS", "EMB"], [reweighted_score_ns, reweighted_score_em]):
+        fig = plt.figure(figsize=(14, 20))
+        for idx, (f, p) in enumerate(
+                zip(reweight_ns['SLy']['features'], score)):
+            title = "chi1 = {0}; chi2 = {1}; SNR = {2}".format(
+                f[0][2], f[0][3], f[0][4])
+            make_plots(
+                f, p, title, (fig, idx+1),
+                prefix='SLy', category=category
+            )
+        plt.savefig("reweighted_" + category + "_param_sweep.png")
+
+
+def make_plots(features, predictions, title, fig_idx,
+               prefix=None, category=None):
+    import matplotlib.pyplot as plt
+    fig_, idx = fig_idx
+    fig_.add_subplot(4, 1, idx)
+    # indices 0 and 1 correspond to mass1 and mass2 respectively
+    plt.scatter(features.T[0], features.T[1],
+                s=10, c=predictions)
+    plt.title(title)
+    plt.tight_layout()
+    plt.colorbar(label='Probability')
+    # plot chirp mass contours
+    m1 = np.linspace(1, 20, 1000)
+    m2 = np.linspace(1, 20, 1000)
+    M1, M2 = np.meshgrid(m1, m2)
+    s1z = np.unique(features.T[2])[0]*np.ones(M1.shape)
+    s2z = np.unique(features.T[3])[0]*np.ones(M2.shape)
+    rem_masses = list()
+    for _ in range(M1.shape[0]):
+        rem_masses.append(
+            computeDiskMass.computeDiskMass(
+                M1[_], M2[_], s1z[_], s2z[_],
+                eosname=prefix
+            )
+        )
+    rem_masses = np.array(rem_masses).reshape(M1.shape)
+    Mc = (M1*M2)**(3./5.)/(M1 + M2)**(1./5.)
+    mask = M1 > M2
+    M1 = np.ma.masked_array(M1, mask=mask)
+    M2 = np.ma.masked_array(M2, mask=mask)
+    s1z = np.ma.masked_array(s1z, mask=mask)
+    s2z = np.ma.masked_array(s2z, mask=mask)
+    Mc = np.ma.masked_array(Mc, mask=mask)
+    rem_masses = np.ma.masked_array(
+        rem_masses, mask=mask*(M2 > EOS_MAX_MASS[prefix])
+    )
+    CS = plt.contour(
+        M1, M2, Mc.T, levels=[2.01, 2.22, 2.99, 3.48, 4.73, 5.4],
+        # (m1, m2) = (4, 1.4) -> Mc = 2.01
+        # (m1, m2) = (5, 1.4) -> Mc = 2.22
+        # (m1, m2) = (10, 1.4) -> Mc = 2.99
+        # (m1, m2) = (4, 4)    -> Mc = 3.48
+        # (m1, m2) = (30, 1.4) -> Mc = 4.73
+        # (m1, m2) = (10, 4)  -> Mc = 5.4
+        # three different NSBH populations;
+        # three different mass-gap populations
+        colors='black', linewidths=1.0
+    )
+    plt.clabel(CS, inline=True, fontsize=16)
+    plt.xlim((1, 20))
+    plt.ylim((1, 12))
+    try:
+        max_mass = EOS_MAX_MASS[prefix]
+    except KeyError:
+        max_mass = 3.0
+    if 'NS' in category:
+        plt.axhline(y=max_mass, c='r', linewidth=1.2)
+    elif 'EM' in category:
+        CS = plt.contour(M1, M2, rem_masses.T,
+                         levels=[0., ], colors='red',
+                         linewidths=1.2)
+    plt.xlabel(r'$m_1$', fontsize=16)
+    plt.ylabel(r'$m_2$', fontsize=16)
+
+
+def run_k_fold_split(features, targets, n_splits=10, random_state=0,
+                     training_task=None, **kwargs):
+    """Split the `features` in `n_splits`, train on `n_splits - 1`
+    sets, test on the last fraction. This performed across the complete
+    dataset.
+
+    Parameters
+    ----------
+    features : numpy.ndarray
+        Feature set
+    targets : numpy.ndarray
+        Target set containing binary classification of `features`
+    n_splits : int
+        Number of splits for `features` and `targets`
+    random_state : int
+        Random seed for the split
+    training_task : callable
+        function with arguments (X_train, y_train, X_test, **kwargs) which
+        trains, and returns predictions on X_test.
+        E.g. :meth:`run_KNN_classifier`,
+        or :meth:`run_RF_classifier`.
+    **kwargs
+        Keyword arguments passed to `training_task`.
+
+    Returns
+    -------
+    tuple
+        (res_predict, res_predict_proba) - predictions and probabilities
+    """
+    res_predict_proba = np.empty(len(features))
+    res_predict = np.empty(len(features))
+    res_predict_proba[:] = np.nan
+    res_predict[:] = np.nan
+
+    sss = KFold(n_splits=n_splits, shuffle=True, random_state=random_state)
+    sss.get_n_splits(features, targets)
+    for train_index, test_index in sss.split(features, targets):
+        X_train, X_test, y_train = \
+            features.iloc[train_index], \
+            features.iloc[test_index], \
+            targets.iloc[train_index]
+
+        predict_proba, predict = training_task(X_train, y_train, X_test,
+                                               **kwargs)
+        # second column is the prob of NS/EMB
+        predict_proba = predict_proba.T[1]
+
+        res_predict_proba[test_index] = predict_proba
+        res_predict[test_index] = predict
+    return res_predict, res_predict_proba
+
+
+def run_KNN_classifier(X_train, y_train,
+                       X_test,
+                       **kwargs):
+    '''
+    Run KNearestNeighborClassifier classifier returns
+    `clf.predict_proba`
+
+    Parameters
+    ----------
+    X_train : numpy.ndarray
+        Feature training set, can be array or Dataframe
+    y_train : numpy.array
+        Target training set, 0 or 1 binary classification
+    X_test : numpy.ndarray
+        Feature testing set, can be array or DataFrame
+    '''
+    if kwargs.get('metric') == 'mahalanobis':
+        kwargs['n_jobs'] = 1  # issue with KDTree, BallTree with n_jobs > 1
+    clf = KNeighborsClassifier(**kwargs)
+    clf.fit(X_train.values, y_train)
+    predictions_proba = clf.predict_proba(X_test)
+    predict = clf.predict(X_test)
+    return predictions_proba, predict
+
+
+def run_RF_classifier(X_train, y_train, X_test,
+                      **kwargs):
+    '''
+    Run RandomForestClassifier; returns
+    `clf.predict_proba`
+
+    Parameters
+    ----------
+    X_train : numpy.ndarray
+        Feature training set, can be array or Dataframe
+    y_train : numpy.array
+        Target training set, 0 or 1 binary classification
+    X_test : numpy.ndarray
+        Feature testing set, can be array or DataFrame
+    '''
+    clf = RandomForestClassifier(**kwargs)
+    clf.fit(X_train.values, y_train)
+    predictions_proba = clf.predict_proba(X_test)
+    predict = clf.predict(X_test)
+    return predictions_proba, predict
```

### Comparing `ligo_em_bright-1.1.3/pyproject.toml` & `ligo_em_bright-1.1.4/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,54 +1,54 @@
-[tool.poetry]
-name = "ligo.em-bright"
-version = "1.1.3"
-description = "Possibility and properties of Electromagnetically-bright sources of gravitational-wave events"
-readme = "README.md"
-authors = [
-    "Deep Chatterjee <deep.chatterjee@ligo.org>",
-    "Shaon Ghosh <shaon.ghosh@ligo.org>"]
-packages = [
-    { include = "ligo" },
-]
-exclude = [
-    "ligo/em_bright/data/*pickle",
-    "ligo/em_bright/data/*json",
-    "ligo/em_bright/data/*dat",
-    "ligo/em_bright/data/*h5"
-]
-license = "MIT"
-
-
-[tool.poetry.dependencies]
-python = ">=3.9"
-scikit-learn = "==1.2.1" 
-astropy = ">=5.2.1"
-pandas = ">=1.5.2"
-lalsuite = "^7.0"
-h5py = ">=3.7.0"
-
-[tool.poetry.dev-dependencies]
-pytest = "*"
-Sphinx = "*"
-toml = "*"
-nbsphinx = "*"
-flake8 = "*"
-htcondor = ">=9.0.6"
-
-
-[tool.poetry.scripts]
-em_bright_categorize = 'ligo.em_bright.categorize:main'
-em_bright_categorize_all_eos = 'ligo.em_bright.categorize:main_all'
-em_bright_create_param_sweep_plot = 'ligo.em_bright.utils:param_sweep_plot'
-em_bright_dag_writer = 'ligo.em_bright.dag_writer:main'
-em_bright_extract = 'ligo.em_bright.utils:extract'
-em_bright_join = 'ligo.em_bright.utils:join'
-em_bright_train = 'ligo.em_bright.utils:train'
-
-
-[tool.pytest.ini_options]
-addopts = "-rsx --tb=short"
-
-
-[build-system]
-requires = ["poetry-core>=1.0.0"]
-build-backend = "poetry.core.masonry.api"
+[tool.poetry]
+name = "ligo.em-bright"
+version = "1.1.4"
+description = "Possibility and properties of Electromagnetically-bright sources of gravitational-wave events"
+readme = "README.md"
+authors = [
+    "Deep Chatterjee <deep.chatterjee@ligo.org>",
+    "Shaon Ghosh <shaon.ghosh@ligo.org>"]
+packages = [
+    { include = "ligo" },
+]
+exclude = [
+    "ligo/em_bright/data/*pickle",
+    "ligo/em_bright/data/*json",
+    "ligo/em_bright/data/*dat",
+    "ligo/em_bright/data/*h5"
+]
+license = "MIT"
+
+
+[tool.poetry.dependencies]
+python = ">=3.9"
+scikit-learn = "==1.2.1" 
+astropy = ">=5.2.1"
+pandas = ">=1.5.2"
+lalsuite = "^7.0"
+h5py = ">=3.7.0"
+
+[tool.poetry.dev-dependencies]
+pytest = "*"
+Sphinx = "*"
+toml = "*"
+nbsphinx = "*"
+flake8 = "*"
+htcondor = ">=9.0.6"
+
+
+[tool.poetry.scripts]
+em_bright_categorize = 'ligo.em_bright.categorize:main'
+em_bright_categorize_all_eos = 'ligo.em_bright.categorize:main_all'
+em_bright_create_param_sweep_plot = 'ligo.em_bright.utils:param_sweep_plot'
+em_bright_dag_writer = 'ligo.em_bright.dag_writer:main'
+em_bright_extract = 'ligo.em_bright.utils:extract'
+em_bright_join = 'ligo.em_bright.utils:join'
+em_bright_train = 'ligo.em_bright.utils:train'
+
+
+[tool.pytest.ini_options]
+addopts = "-rsx --tb=short"
+
+
+[build-system]
+requires = ["poetry-core>=1.0.0"]
+build-backend = "poetry.core.masonry.api"
```

### Comparing `ligo_em_bright-1.1.3/PKG-INFO` & `ligo_em_bright-1.1.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ligo-em-bright
-Version: 1.1.3
+Version: 1.1.4
 Summary: Possibility and properties of Electromagnetically-bright sources of gravitational-wave events
 License: MIT
 Author: Deep Chatterjee
 Author-email: deep.chatterjee@ligo.org
 Requires-Python: >=3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

