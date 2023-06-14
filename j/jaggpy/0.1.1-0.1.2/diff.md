# Comparing `tmp/jaggpy-0.1.1.tar.gz` & `tmp/jaggpy-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/ronald/Documents/Veni/programming/jaggpy/dist/tmply2lvuol/jaggpy-0.1.1.tar", last modified: Mon Nov  1 13:34:30 2021, max compression
+gzip compressed data, was "jaggpy-0.1.2.tar", last modified: Wed Jun 14 15:19:26 2023, max compression
```

## Comparing `jaggpy-0.1.1.tar` & `jaggpy-0.1.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2021-11-01 13:34:30.000000 jaggpy-0.1.1/
--rw-r--r--   0 ronald     (501) staff       (20)     1071 2021-09-27 07:26:51.000000 jaggpy-0.1.1/LICENSE
--rw-r--r--   0 ronald     (501) staff       (20)    11050 2021-11-01 13:34:30.000000 jaggpy-0.1.1/PKG-INFO
--rw-r--r--   0 ronald     (501) staff       (20)    10506 2021-11-01 13:28:22.000000 jaggpy-0.1.1/README.md
--rw-r--r--   0 ronald     (501) staff       (20)      105 2021-10-28 14:03:30.000000 jaggpy-0.1.1/pyproject.toml
--rw-r--r--   0 ronald     (501) staff       (20)      706 2021-11-01 13:34:30.000000 jaggpy-0.1.1/setup.cfg
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2021-11-01 13:34:30.000000 jaggpy-0.1.1/src/
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2021-11-01 13:34:30.000000 jaggpy-0.1.1/src/jaggpy/
--rw-r--r--   0 ronald     (501) staff       (20)      131 2021-11-01 11:14:17.000000 jaggpy-0.1.1/src/jaggpy/__init__.py
--rw-r--r--   0 ronald     (501) staff       (20)     9828 2021-11-01 13:24:14.000000 jaggpy-0.1.1/src/jaggpy/asp_solver.py
--rw-r--r--   0 ronald     (501) staff       (20)    11423 2021-11-01 13:23:33.000000 jaggpy-0.1.1/src/jaggpy/bf_solver.py
--rw-r--r--   0 ronald     (501) staff       (20)     9858 2021-11-01 13:23:21.000000 jaggpy-0.1.1/src/jaggpy/classes.py
--rw-r--r--   0 ronald     (501) staff       (20)    10440 2021-10-29 13:48:41.000000 jaggpy-0.1.1/src/jaggpy/parser.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2021-11-01 13:34:30.000000 jaggpy-0.1.1/src/jaggpy/tests/
--rw-r--r--   0 ronald     (501) staff       (20)       88 2021-11-01 13:06:27.000000 jaggpy-0.1.1/src/jaggpy/tests/__init__.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2021-11-01 13:34:30.000000 jaggpy-0.1.1/src/jaggpy/tests/files/
--rw-r--r--   0 ronald     (501) staff       (20)      867 2021-11-01 12:20:42.000000 jaggpy-0.1.1/src/jaggpy/tests/files/scenario1.jagg
--rw-r--r--   0 ronald     (501) staff       (20)     1892 2021-11-01 13:24:30.000000 jaggpy-0.1.1/src/jaggpy/tests/test_asp.py
--rw-r--r--   0 ronald     (501) staff       (20)     1604 2021-11-01 13:24:34.000000 jaggpy-0.1.1/src/jaggpy/tests/test_bf.py
-drwxr-xr-x   0 ronald     (501) staff       (20)        0 2021-11-01 13:34:30.000000 jaggpy-0.1.1/src/jaggpy.egg-info/
--rw-r--r--   0 ronald     (501) staff       (20)    11050 2021-11-01 13:34:30.000000 jaggpy-0.1.1/src/jaggpy.egg-info/PKG-INFO
--rw-r--r--   0 ronald     (501) staff       (20)      450 2021-11-01 13:34:30.000000 jaggpy-0.1.1/src/jaggpy.egg-info/SOURCES.txt
--rw-r--r--   0 ronald     (501) staff       (20)        1 2021-11-01 13:34:30.000000 jaggpy-0.1.1/src/jaggpy.egg-info/dependency_links.txt
--rw-r--r--   0 ronald     (501) staff       (20)       21 2021-11-01 13:34:30.000000 jaggpy-0.1.1/src/jaggpy.egg-info/requires.txt
--rw-r--r--   0 ronald     (501) staff       (20)        7 2021-11-01 13:34:30.000000 jaggpy-0.1.1/src/jaggpy.egg-info/top_level.txt
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-14 15:19:26.795810 jaggpy-0.1.2/
+-rw-r--r--   0 ronald     (501) staff       (20)     1071 2021-09-27 07:26:51.000000 jaggpy-0.1.2/LICENSE
+-rw-r--r--   0 ronald     (501) staff       (20)    10974 2023-06-14 15:19:26.794957 jaggpy-0.1.2/PKG-INFO
+-rw-r--r--   0 ronald     (501) staff       (20)    10506 2023-06-14 14:26:08.000000 jaggpy-0.1.2/README.md
+-rw-r--r--   0 ronald     (501) staff       (20)      902 2023-06-14 15:16:49.000000 jaggpy-0.1.2/pyproject.toml
+-rw-r--r--   0 ronald     (501) staff       (20)       38 2023-06-14 15:19:26.795900 jaggpy-0.1.2/setup.cfg
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-14 15:19:26.783925 jaggpy-0.1.2/src/
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-14 15:19:26.789541 jaggpy-0.1.2/src/jaggpy/
+-rw-r--r--   0 ronald     (501) staff       (20)      131 2021-11-01 11:14:17.000000 jaggpy-0.1.2/src/jaggpy/__init__.py
+-rw-r--r--   0 ronald     (501) staff       (20)     9865 2023-06-14 15:00:32.000000 jaggpy-0.1.2/src/jaggpy/asp_solver.py
+-rw-r--r--   0 ronald     (501) staff       (20)    11420 2023-06-14 14:59:38.000000 jaggpy-0.1.2/src/jaggpy/bf_solver.py
+-rw-r--r--   0 ronald     (501) staff       (20)    10043 2023-06-14 14:57:09.000000 jaggpy-0.1.2/src/jaggpy/classes.py
+-rw-r--r--   0 ronald     (501) staff       (20)    10426 2023-06-14 14:57:18.000000 jaggpy-0.1.2/src/jaggpy/parser.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-14 15:19:26.793610 jaggpy-0.1.2/src/jaggpy/tests/
+-rw-r--r--   0 ronald     (501) staff       (20)       88 2021-11-01 13:06:27.000000 jaggpy-0.1.2/src/jaggpy/tests/__init__.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-14 15:19:26.794341 jaggpy-0.1.2/src/jaggpy/tests/files/
+-rw-r--r--   0 ronald     (501) staff       (20)      867 2021-11-01 12:20:42.000000 jaggpy-0.1.2/src/jaggpy/tests/files/scenario1.jagg
+-rw-r--r--   0 ronald     (501) staff       (20)     1892 2021-11-01 13:24:30.000000 jaggpy-0.1.2/src/jaggpy/tests/test_asp.py
+-rw-r--r--   0 ronald     (501) staff       (20)     1604 2021-11-01 13:24:34.000000 jaggpy-0.1.2/src/jaggpy/tests/test_bf.py
+drwxr-xr-x   0 ronald     (501) staff       (20)        0 2023-06-14 15:19:26.791974 jaggpy-0.1.2/src/jaggpy.egg-info/
+-rw-r--r--   0 ronald     (501) staff       (20)    10974 2023-06-14 15:19:26.000000 jaggpy-0.1.2/src/jaggpy.egg-info/PKG-INFO
+-rw-r--r--   0 ronald     (501) staff       (20)      440 2023-06-14 15:19:26.000000 jaggpy-0.1.2/src/jaggpy.egg-info/SOURCES.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        1 2023-06-14 15:19:26.000000 jaggpy-0.1.2/src/jaggpy.egg-info/dependency_links.txt
+-rw-r--r--   0 ronald     (501) staff       (20)       21 2023-06-14 15:19:26.000000 jaggpy-0.1.2/src/jaggpy.egg-info/requires.txt
+-rw-r--r--   0 ronald     (501) staff       (20)        7 2023-06-14 15:19:26.000000 jaggpy-0.1.2/src/jaggpy.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `jaggpy-0.1.1/LICENSE` & `jaggpy-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `jaggpy-0.1.1/PKG-INFO` & `jaggpy-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,17 @@
 Metadata-Version: 2.1
 Name: jaggpy
-Version: 0.1.1
+Version: 0.1.2
 Summary: A Python package for Judgment Aggregation
-Home-page: https://github.com/rdehaan/jaggpy
-Author: Ronald de Haan, Bo Flachs, Philemon Huising
-Author-email: me@ronalddehaan.eu
-License: UNKNOWN
-Platform: UNKNOWN
+Maintainer-email: Ronald de Haan <me@ronalddehaan.eu>
+Project-URL: repository, https://github.com/rdehaan/jaggpy/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering
-Requires-Python: >=3.4
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # JAGGPY
 
 `jaggpy` is a Python package for computing outcomes of [judgment aggregation](https://plato.stanford.edu/entries/belief-merging/#JudAgg) (JA) scenarios. The package allows for JA scenarios in the most general form, where issues in the agenda, constraints on judgment sets and constraints on the outcome may be arbitrary formulas. For more information on the formal framework used see, e.g.,
 > Endriss, U., de Haan, R., Lang, J., & Slavkovik, M. (2020). [The Complexity Landscape of Outcome Determination in Judgment Aggregation](https://doi.org/10.1613/jair.1.11970). *Journal of Artificial Intelligence Research*, *69*, 687-731.
@@ -234,9 +230,7 @@
 Github Link: [https://github.com/rdehaan/jaggpy](https://github.com/rdehaan/jaggpy)
 
 
 <!-- REFERENCES -->
 ## References
 - Endriss, U., de Haan, R., Lang, J., & Slavkovik, M. (2020). [The Complexity Landscape of Outcome Determination in Judgment Aggregation](https://doi.org/10.1613/jair.1.11970). *Journal of Artificial Intelligence Research*, *69*, 687-731.
 - de Haan, R., & Slavkovik, M. (2019). [Answer set programming for judgment aggregation](https://doi.org/10.24963/ijcai.2019/231). In *Proceedings of the 28th International Joint Conference on Artificial Intelligence (IJCAI 2019)*. AAAI Press.
-
-
```

#### html2text {}

```diff
@@ -1,31 +1,31 @@
-Metadata-Version: 2.1 Name: jaggpy Version: 0.1.1 Summary: A Python package for
-Judgment Aggregation Home-page: https://github.com/rdehaan/jaggpy Author:
-Ronald de Haan, Bo Flachs, Philemon Huising Author-email: me@ronalddehaan.eu
-License: UNKNOWN Platform: UNKNOWN Classifier: Programming Language :: Python
-:: 3 Classifier: License :: OSI Approved :: MIT License Classifier: Operating
-System :: OS Independent Classifier: Topic :: Scientific/Engineering Requires-
-Python: >=3.4 Description-Content-Type: text/markdown License-File: LICENSE #
-JAGGPY `jaggpy` is a Python package for computing outcomes of [judgment
-aggregation](https://plato.stanford.edu/entries/belief-merging/#JudAgg) (JA)
-scenarios. The package allows for JA scenarios in the most general form, where
-issues in the agenda, constraints on judgment sets and constraints on the
-outcome may be arbitrary formulas. For more information on the formal framework
-used see, e.g., > Endriss, U., de Haan, R., Lang, J., & Slavkovik, M. (2020).
-[The Complexity Landscape of Outcome Determination in Judgment Aggregation]
-(https://doi.org/10.1613/jair.1.11970). *Journal of Artificial Intelligence
-Research*, *69*, 687-731. in which it is referred to as *framework (6)*. The
-package offers two ways in which to generate outcomes for a scenario given a JA
-rule. The first (and slowest) is a brute force solver, and the second makes use
-of Answer Set Programming (ASP) for the efficient computation of outcomes,
-building on the encodings presented by de Haan and Slavkovik in > de Haan, R.,
-& Slavkovik, M. (2019). [Answer set programming for judgment aggregation]
-(https://doi.org/10.24963/ijcai.2019/231). In *Proceedings of the 28th
-International Joint Conference on Artificial Intelligence (IJCAI 2019)*. AAAI
-Press.  ## Table of contents
+Metadata-Version: 2.1 Name: jaggpy Version: 0.1.2 Summary: A Python package for
+Judgment Aggregation Maintainer-email: Ronald de Haan
+ronalddehaan.eu> Project-URL: repository, https://github.com/rdehaan/jaggpy/
+Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
+Approved :: MIT License Classifier: Operating System :: OS Independent
+Classifier: Topic :: Scientific/Engineering Description-Content-Type: text/
+markdown License-File: LICENSE # JAGGPY `jaggpy` is a Python package for
+computing outcomes of [judgment aggregation](https://plato.stanford.edu/
+entries/belief-merging/#JudAgg) (JA) scenarios. The package allows for JA
+scenarios in the most general form, where issues in the agenda, constraints on
+judgment sets and constraints on the outcome may be arbitrary formulas. For
+more information on the formal framework used see, e.g., > Endriss, U., de
+Haan, R., Lang, J., & Slavkovik, M. (2020). [The Complexity Landscape of
+Outcome Determination in Judgment Aggregation](https://doi.org/10.1613/
+jair.1.11970). *Journal of Artificial Intelligence Research*, *69*, 687-731. in
+which it is referred to as *framework (6)*. The package offers two ways in
+which to generate outcomes for a scenario given a JA rule. The first (and
+slowest) is a brute force solver, and the second makes use of Answer Set
+Programming (ASP) for the efficient computation of outcomes, building on the
+encodings presented by de Haan and Slavkovik in > de Haan, R., & Slavkovik, M.
+(2019). [Answer set programming for judgment aggregation](https://doi.org/
+10.24963/ijcai.2019/231). In *Proceedings of the 28th International Joint
+Conference on Artificial Intelligence (IJCAI 2019)*. AAAI Press.  ## Table of
+contents
    1. Getting_started
           o Prerequisites
           o Installation
           o Tests
    2. Usage
           o Scenario_objects
                 # Formulas
```

### Comparing `jaggpy-0.1.1/README.md` & `jaggpy-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `jaggpy-0.1.1/src/jaggpy/asp_solver.py` & `jaggpy-0.1.2/src/jaggpy/asp_solver.py`

 * *Files 0% similar despite different names*

```diff
@@ -156,57 +156,57 @@
         agent(col).
         :- agent(col), outputClause(C,_), js(col,-L) : outputClause(C,L).
         """)
 
         # Add the ASP code corresponding to the rule that is to be executed.
         if rule == "kemeny":
             if verbose:
-                print("Computing outcome with ASP and the Kemeny rule...")
+                print("Computing outcomes with ASP and the Kemeny rule...")
             asp_program += textwrap.dedent("""
             % Kemeny rule
             wgt(X,N) :- lit(X), N = #count { A : voter(A), js(A,X) }.
             #maximize { N@1,wgt(X,N) : wgt(X,N), js(col,X) }.
             """)
 
         elif rule == "leximax":
             if verbose:
-                print("Computing outcome with ASP and the Leximax rule...")
+                print("Computing outcomes with ASP and the Leximax rule...")
             asp_program += textwrap.dedent("""
             % Leximax rule
             wgt(X,N) :- lit(X), N = #count { A : voter(A), js(A,X) }.
             #maximize { 1@N,wgt(X,N) : wgt(X,N), js(col,X) }.
             """)
 
         elif rule == "young":
             if verbose:
-                print("Computing outcome with ASP and the Young rule...")
+                print("Computing outcomes with ASP and the Young rule...")
             asp_program += textwrap.dedent("""
             % Young rule
             in(A) ; out(A) :- voter(A).
             inwgt(X,N) :- lit(X), N = #count{ A : voter(A), in(A), js(A,X) }.
             inmaj(X) :- lit(X), inwgt(X,N), inwgt(-X,M), N > M.
             js(col,X) :- inmaj(X).
             #minimize { 1@1,out(A) : out(A) }.
             """)
 
         elif rule == "slater":
             if verbose:
-                print("Computing outcome with ASP and the Slater rule...")
+                print("Computing outcomes with ASP and the Slater rule...")
             asp_program += textwrap.dedent("""
             % Slater rule
             % determine the majority outcome
             pc(X,N) :- lit(X), N = #count { A : voter(A), js(A,X) }.
             maj(X) :- lit(X), pc(X,N), pc(-X,M), N > M.
             % maximize agreement with the majority outcome
             #minimize { 1@10,maj(X) : maj(X), js(col,-X) }.
             """)
 
         elif rule == "majority":
             if verbose:
-                print("Computing outcome with ASP and the Majority rule...")
+                print("Computing outcomes with ASP and the Majority rule...")
             asp_program += textwrap.dedent("""
             % Majority rule
             % require that the collective outcome agrees with all issues
             % that have strictly more support than their negation
             pc(X,N) :- lit(X), N = #count { A : voter(A), js(A,X) }.
             maj(X) :- lit(X), pc(X,N), pc(-X,M), N > M.
             js(col,X) :- maj(X).
@@ -217,14 +217,15 @@
         # Add the outcome predicate.
         asp_program += textwrap.dedent("""
             outcome(X) :- agent(col), js(col, X), issue(X).
             #show outcome/1.
                 """)
 
         # Ground and solve the program.
+        # pylint: disable=E1101
         control = clingo.Control(arguments=["--project"])
         control.add("base", [], asp_program)
         control.ground([("base", [])])
         control.configuration.solve.models = 0
         control.configuration.solve.opt_mode = "optN"
 
         # Yield the results of the program.
```

### Comparing `jaggpy-0.1.1/src/jaggpy/bf_solver.py` & `jaggpy-0.1.2/src/jaggpy/bf_solver.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,42 +46,42 @@
 
         # Make sure that each variable gets an assignment.
         for var in all_variables:
             my_string += f"({var} | ~{var}) & "
         my_string = my_string[:-3]
 
         # Preprocess the string representing the scenario.
-        var_prefix = "my_var_"
+        var_prefix = "_"
         my_string_preprocessed = my_string
         for var in all_variables:
             my_string_preprocessed = my_string_preprocessed.replace(var, var_prefix + var)
         for var in all_variables:
             exec(f"{var_prefix}{var} = Var('{var}')")
         output_contstraint = eval(my_string_preprocessed)
 
         # List all the models that are consistent with the output constraints.
         consistent_outcomes =  list(output_contstraint.models())
 
         # We determine the outcome with a helper function that corresponds to the chosen rule.
         # Kemeny rule
         if rule == "kemeny":
             if verbose:
-                print("Computing outcome with the brute force solver and the Kemeny rule...")
+                print("Computing outcomes with the brute force solver and the Kemeny rule...")
             outcomes = self.solve_kemeny(scenario, consistent_outcomes)
 
         # MaxHamming rule
         elif rule == "maxhamming":
             if verbose:
-                print("Computing outcome with the brute force solver and the MaxHamming rule...")
+                print("Computing outcomes with the brute force solver and the MaxHamming rule...")
             outcomes =  self.solve_max_hamming(scenario, consistent_outcomes)
 
         # Slater rule
         elif rule == "slater":
             if verbose:
-                print("Computing outcome with the brute force solver and the Slater rule...")
+                print("Computing outcomes with the brute force solver and the Slater rule...")
             outcomes = self.solve_slater(scenario, consistent_outcomes)
 
         else:
             raise Exception (f"{rule} is not a recognized aggregation rule.")
 
         # Clean outcomes to only contain issues
         for i, outcome in enumerate(outcomes):
```

### Comparing `jaggpy-0.1.1/src/jaggpy/classes.py` & `jaggpy-0.1.2/src/jaggpy/classes.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,14 +69,16 @@
         lines = [line for line in lines if line != "" and line[0] != "#"]
 
         # Create a parser object for future use
         parser = Parser()
 
         # Add the variables to the scenario
         self.variables = lines[0].split(", ")
+        # Remove duplicates
+        self.variables = list(set(self.variables))
 
         # Add the formulas to the agenda dictionary using the given label
         number_of_formulass = int(lines[1])
         for i in range(2, number_of_formulass+2):
             current_line = lines[i].split(", ")
             label = int(current_line[0])
             formula = current_line[1]
@@ -136,37 +138,40 @@
                 # Check consistency of the judgment set with respect
                 # to the input constraint
                 my_string = ""
                 for conjunct in self.input_constraints:
                     my_string += f"({conjunct}) & "
                 for j in range(1, len(self.agenda)+1):
                     if j not in formula_labels:
-                        my_string += f"(~{self.agenda[j]}) & "
+                        nnf_formula = parser.to_nnf(f"~{self.agenda[j]}")
+                        my_string += f"({nnf_formula}) & "
                     else:
                         my_string += f"({self.agenda[j]}) & "
                 my_string = my_string[:-3]
                 self.check_consistency(my_string)
                 if not self.check_consistency(my_string):
                     raise Exception (f"The judgment set on line {i} is inconsistent"\
                         " with the input constraints.")
 
                 # Add the judgment set to the scenario
                 self.profile.append([label, accepted_formulas])
             else:
                 # If the all issues are rejected, add the empty list
+                label = int(current_line[0])
                 self.profile.append([label, []])
 
+
     def check_consistency(self, sentence):
         """The function check_consistency should receive an NNF-formula as a
         string. It return a Boolean indicating whether the formula is consistent."""
         my_string = sentence
 
         # Use a prefix to prevent variable name collisions
         # Add this prefix to all variables in the string
-        var_prefix = "my_var_"
+        var_prefix = "_"
         my_string_preprocessed = my_string
         for var in self.variables:
             my_string_preprocessed = my_string_preprocessed.replace(var, var_prefix + var)
 
         # Declare variables (with prefix) and parse the formula with the
         # variable prefixes added
         for var in self.variables:
@@ -178,15 +183,15 @@
 
 
     def pretty_repr(self):
         """Returns string that represents the scenario object in a readable way"""
         scenario_string = "Variables:"
         for variable in self.variables:
             scenario_string += f"\n{variable}"
-        scenario_string += "\n\nSub-agenda (label, formula):"
+        scenario_string += "\n\nAgenda (label, formula):"
         for key in self.agenda:
             scenario_string += f"\n{key}, {self.agenda[key]}"
         scenario_string += "\n\nInput constraints:"
         for constraint in self.input_constraints:
             scenario_string += f"\n{constraint}"
         scenario_string +=  "\n\nOutput constraints:"
         for constraint in self.output_constraints:
```

### Comparing `jaggpy-0.1.1/src/jaggpy/parser.py` & `jaggpy-0.1.2/src/jaggpy/parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -211,15 +211,15 @@
         an updated list of all occurring variables.
         """
         my_string = sentence
         all_variables = set()
 
         # Use a prefix to prevent variable name collisions
         # Add this prefix to all variables in the string
-        var_prefix = "my_var_"
+        var_prefix = "_"
         my_string_preprocessed = my_string
         for var in variables:
             my_string_preprocessed = my_string_preprocessed.replace(var, var_prefix + var)
 
         # Declare variables (with prefix) and parse the formula with the
         # variable prefixes added
         for var in variables:
@@ -273,8 +273,7 @@
             new_constraints.append(f'~{label_var} | {formula}')
 
             # Add formula -> label
             neg_formula = self.to_nnf(f'~ ({formula})')
             new_constraints.append(f'{neg_formula} | {label_var}')
 
         return new_constraints
-
```

### Comparing `jaggpy-0.1.1/src/jaggpy/tests/files/scenario1.jagg` & `jaggpy-0.1.2/src/jaggpy/tests/files/scenario1.jagg`

 * *Files identical despite different names*

### Comparing `jaggpy-0.1.1/src/jaggpy/tests/test_asp.py` & `jaggpy-0.1.2/src/jaggpy/tests/test_asp.py`

 * *Files identical despite different names*

### Comparing `jaggpy-0.1.1/src/jaggpy/tests/test_bf.py` & `jaggpy-0.1.2/src/jaggpy/tests/test_bf.py`

 * *Files identical despite different names*

### Comparing `jaggpy-0.1.1/src/jaggpy.egg-info/PKG-INFO` & `jaggpy-0.1.2/src/jaggpy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,17 @@
 Metadata-Version: 2.1
 Name: jaggpy
-Version: 0.1.1
+Version: 0.1.2
 Summary: A Python package for Judgment Aggregation
-Home-page: https://github.com/rdehaan/jaggpy
-Author: Ronald de Haan, Bo Flachs, Philemon Huising
-Author-email: me@ronalddehaan.eu
-License: UNKNOWN
-Platform: UNKNOWN
+Maintainer-email: Ronald de Haan <me@ronalddehaan.eu>
+Project-URL: repository, https://github.com/rdehaan/jaggpy/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering
-Requires-Python: >=3.4
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # JAGGPY
 
 `jaggpy` is a Python package for computing outcomes of [judgment aggregation](https://plato.stanford.edu/entries/belief-merging/#JudAgg) (JA) scenarios. The package allows for JA scenarios in the most general form, where issues in the agenda, constraints on judgment sets and constraints on the outcome may be arbitrary formulas. For more information on the formal framework used see, e.g.,
 > Endriss, U., de Haan, R., Lang, J., & Slavkovik, M. (2020). [The Complexity Landscape of Outcome Determination in Judgment Aggregation](https://doi.org/10.1613/jair.1.11970). *Journal of Artificial Intelligence Research*, *69*, 687-731.
@@ -234,9 +230,7 @@
 Github Link: [https://github.com/rdehaan/jaggpy](https://github.com/rdehaan/jaggpy)
 
 
 <!-- REFERENCES -->
 ## References
 - Endriss, U., de Haan, R., Lang, J., & Slavkovik, M. (2020). [The Complexity Landscape of Outcome Determination in Judgment Aggregation](https://doi.org/10.1613/jair.1.11970). *Journal of Artificial Intelligence Research*, *69*, 687-731.
 - de Haan, R., & Slavkovik, M. (2019). [Answer set programming for judgment aggregation](https://doi.org/10.24963/ijcai.2019/231). In *Proceedings of the 28th International Joint Conference on Artificial Intelligence (IJCAI 2019)*. AAAI Press.
-
-
```

#### html2text {}

```diff
@@ -1,31 +1,31 @@
-Metadata-Version: 2.1 Name: jaggpy Version: 0.1.1 Summary: A Python package for
-Judgment Aggregation Home-page: https://github.com/rdehaan/jaggpy Author:
-Ronald de Haan, Bo Flachs, Philemon Huising Author-email: me@ronalddehaan.eu
-License: UNKNOWN Platform: UNKNOWN Classifier: Programming Language :: Python
-:: 3 Classifier: License :: OSI Approved :: MIT License Classifier: Operating
-System :: OS Independent Classifier: Topic :: Scientific/Engineering Requires-
-Python: >=3.4 Description-Content-Type: text/markdown License-File: LICENSE #
-JAGGPY `jaggpy` is a Python package for computing outcomes of [judgment
-aggregation](https://plato.stanford.edu/entries/belief-merging/#JudAgg) (JA)
-scenarios. The package allows for JA scenarios in the most general form, where
-issues in the agenda, constraints on judgment sets and constraints on the
-outcome may be arbitrary formulas. For more information on the formal framework
-used see, e.g., > Endriss, U., de Haan, R., Lang, J., & Slavkovik, M. (2020).
-[The Complexity Landscape of Outcome Determination in Judgment Aggregation]
-(https://doi.org/10.1613/jair.1.11970). *Journal of Artificial Intelligence
-Research*, *69*, 687-731. in which it is referred to as *framework (6)*. The
-package offers two ways in which to generate outcomes for a scenario given a JA
-rule. The first (and slowest) is a brute force solver, and the second makes use
-of Answer Set Programming (ASP) for the efficient computation of outcomes,
-building on the encodings presented by de Haan and Slavkovik in > de Haan, R.,
-& Slavkovik, M. (2019). [Answer set programming for judgment aggregation]
-(https://doi.org/10.24963/ijcai.2019/231). In *Proceedings of the 28th
-International Joint Conference on Artificial Intelligence (IJCAI 2019)*. AAAI
-Press.  ## Table of contents
+Metadata-Version: 2.1 Name: jaggpy Version: 0.1.2 Summary: A Python package for
+Judgment Aggregation Maintainer-email: Ronald de Haan
+ronalddehaan.eu> Project-URL: repository, https://github.com/rdehaan/jaggpy/
+Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
+Approved :: MIT License Classifier: Operating System :: OS Independent
+Classifier: Topic :: Scientific/Engineering Description-Content-Type: text/
+markdown License-File: LICENSE # JAGGPY `jaggpy` is a Python package for
+computing outcomes of [judgment aggregation](https://plato.stanford.edu/
+entries/belief-merging/#JudAgg) (JA) scenarios. The package allows for JA
+scenarios in the most general form, where issues in the agenda, constraints on
+judgment sets and constraints on the outcome may be arbitrary formulas. For
+more information on the formal framework used see, e.g., > Endriss, U., de
+Haan, R., Lang, J., & Slavkovik, M. (2020). [The Complexity Landscape of
+Outcome Determination in Judgment Aggregation](https://doi.org/10.1613/
+jair.1.11970). *Journal of Artificial Intelligence Research*, *69*, 687-731. in
+which it is referred to as *framework (6)*. The package offers two ways in
+which to generate outcomes for a scenario given a JA rule. The first (and
+slowest) is a brute force solver, and the second makes use of Answer Set
+Programming (ASP) for the efficient computation of outcomes, building on the
+encodings presented by de Haan and Slavkovik in > de Haan, R., & Slavkovik, M.
+(2019). [Answer set programming for judgment aggregation](https://doi.org/
+10.24963/ijcai.2019/231). In *Proceedings of the 28th International Joint
+Conference on Artificial Intelligence (IJCAI 2019)*. AAAI Press.  ## Table of
+contents
    1. Getting_started
           o Prerequisites
           o Installation
           o Tests
    2. Usage
           o Scenario_objects
                 # Formulas
```

