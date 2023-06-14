# Comparing `tmp/ProjectAssessment-0.2.9.tar.gz` & `tmp/ProjectAssessment-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ProjectAssessment-0.2.9.tar", last modified: Fri Nov 25 12:57:07 2022, max compression
+gzip compressed data, was "ProjectAssessment-0.3.0.tar", last modified: Wed Jun 14 20:04:59 2023, max compression
```

## Comparing `ProjectAssessment-0.2.9.tar` & `ProjectAssessment-0.3.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 tazz       (501) staff       (20)        0 2022-11-25 12:57:07.581640 ProjectAssessment-0.2.9/
--rw-r--r--   0 tazz       (501) staff       (20)     1066 2022-06-04 12:11:30.000000 ProjectAssessment-0.2.9/LICENSE
--rw-r--r--   0 tazz       (501) staff       (20)      831 2022-11-25 12:57:07.581538 ProjectAssessment-0.2.9/PKG-INFO
-drwxr-xr-x   0 tazz       (501) staff       (20)        0 2022-11-25 12:57:07.580773 ProjectAssessment-0.2.9/ProjectAssessment/
--rw-r--r--   0 tazz       (501) staff       (20)       99 2022-06-29 18:35:17.000000 ProjectAssessment-0.2.9/ProjectAssessment/MakeTable.py
--rw-r--r--   0 tazz       (501) staff       (20)     3614 2022-11-17 18:51:56.000000 ProjectAssessment-0.2.9/ProjectAssessment/Marginal.py
--rw-r--r--   0 tazz       (501) staff       (20)    17670 2022-11-25 12:50:41.000000 ProjectAssessment-0.2.9/ProjectAssessment/Solver.py
--rw-r--r--   0 tazz       (501) staff       (20)       83 2022-11-25 12:54:32.000000 ProjectAssessment-0.2.9/ProjectAssessment/__init__.py
-drwxr-xr-x   0 tazz       (501) staff       (20)        0 2022-11-25 12:57:07.581374 ProjectAssessment-0.2.9/ProjectAssessment.egg-info/
--rw-r--r--   0 tazz       (501) staff       (20)      831 2022-11-25 12:57:07.000000 ProjectAssessment-0.2.9/ProjectAssessment.egg-info/PKG-INFO
--rw-r--r--   0 tazz       (501) staff       (20)      349 2022-11-25 12:57:07.000000 ProjectAssessment-0.2.9/ProjectAssessment.egg-info/SOURCES.txt
--rw-r--r--   0 tazz       (501) staff       (20)        1 2022-11-25 12:57:07.000000 ProjectAssessment-0.2.9/ProjectAssessment.egg-info/dependency_links.txt
--rw-r--r--   0 tazz       (501) staff       (20)       60 2022-11-25 12:57:07.000000 ProjectAssessment-0.2.9/ProjectAssessment.egg-info/requires.txt
--rw-r--r--   0 tazz       (501) staff       (20)       18 2022-11-25 12:57:07.000000 ProjectAssessment-0.2.9/ProjectAssessment.egg-info/top_level.txt
--rw-r--r--   0 tazz       (501) staff       (20)     5067 2022-11-16 14:03:18.000000 ProjectAssessment-0.2.9/README.md
--rw-r--r--   0 tazz       (501) staff       (20)       38 2022-11-25 12:57:07.581679 ProjectAssessment-0.2.9/setup.cfg
--rw-r--r--   0 tazz       (501) staff       (20)     1082 2022-11-25 12:54:42.000000 ProjectAssessment-0.2.9/setup.py
+drwxr-xr-x   0 tazz       (501) staff       (20)        0 2023-06-14 20:04:59.928745 ProjectAssessment-0.3.0/
+-rw-r--r--   0 tazz       (501) staff       (20)     1066 2022-06-04 12:11:30.000000 ProjectAssessment-0.3.0/LICENSE
+-rw-r--r--   0 tazz       (501) staff       (20)      831 2023-06-14 20:04:59.928652 ProjectAssessment-0.3.0/PKG-INFO
+drwxr-xr-x   0 tazz       (501) staff       (20)        0 2023-06-14 20:04:59.927766 ProjectAssessment-0.3.0/ProjectAssessment/
+-rw-r--r--   0 tazz       (501) staff       (20)       99 2022-06-29 18:35:17.000000 ProjectAssessment-0.3.0/ProjectAssessment/MakeTable.py
+-rw-r--r--   0 tazz       (501) staff       (20)     4659 2023-06-14 19:59:55.000000 ProjectAssessment-0.3.0/ProjectAssessment/Marginal.py
+-rw-r--r--   0 tazz       (501) staff       (20)    21282 2023-06-14 19:59:55.000000 ProjectAssessment-0.3.0/ProjectAssessment/Solver.py
+-rw-r--r--   0 tazz       (501) staff       (20)       84 2022-12-16 11:54:15.000000 ProjectAssessment-0.3.0/ProjectAssessment/__init__.py
+drwxr-xr-x   0 tazz       (501) staff       (20)        0 2023-06-14 20:04:59.928504 ProjectAssessment-0.3.0/ProjectAssessment.egg-info/
+-rw-r--r--   0 tazz       (501) staff       (20)      831 2023-06-14 20:04:59.000000 ProjectAssessment-0.3.0/ProjectAssessment.egg-info/PKG-INFO
+-rw-r--r--   0 tazz       (501) staff       (20)      349 2023-06-14 20:04:59.000000 ProjectAssessment-0.3.0/ProjectAssessment.egg-info/SOURCES.txt
+-rw-r--r--   0 tazz       (501) staff       (20)        1 2023-06-14 20:04:59.000000 ProjectAssessment-0.3.0/ProjectAssessment.egg-info/dependency_links.txt
+-rw-r--r--   0 tazz       (501) staff       (20)       60 2023-06-14 20:04:59.000000 ProjectAssessment-0.3.0/ProjectAssessment.egg-info/requires.txt
+-rw-r--r--   0 tazz       (501) staff       (20)       18 2023-06-14 20:04:59.000000 ProjectAssessment-0.3.0/ProjectAssessment.egg-info/top_level.txt
+-rw-r--r--   0 tazz       (501) staff       (20)     6770 2023-06-14 19:59:55.000000 ProjectAssessment-0.3.0/README.md
+-rw-r--r--   0 tazz       (501) staff       (20)       38 2023-06-14 20:04:59.928781 ProjectAssessment-0.3.0/setup.cfg
+-rw-r--r--   0 tazz       (501) staff       (20)     1082 2023-06-14 19:59:55.000000 ProjectAssessment-0.3.0/setup.py
```

### Comparing `ProjectAssessment-0.2.9/LICENSE` & `ProjectAssessment-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ProjectAssessment-0.2.9/PKG-INFO` & `ProjectAssessment-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: ProjectAssessment
-Version: 0.2.9
+Version: 0.3.0
 Summary: Package to compute the Project-Based Assessment estimates of student and rubric proficiency.
 Home-page: https://github.com/tazzben/project-based-assessment
-Download-URL: https://github.com/tazzben/project-based-assessment/archive/v0.2.9.tar.gz
+Download-URL: https://github.com/tazzben/project-based-assessment/archive/v0.3.0.tar.gz
 Author: Ben Smith
 Author-email: bosmith@unomaha.edu
 License: MIT
 Keywords: Assessment,Projects,Statistics,Education,Bootstrap
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ProjectAssessment-0.2.9/ProjectAssessment/Marginal.py` & `ProjectAssessment-0.3.0/ProjectAssessment/Marginal.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,14 +3,27 @@
 import pandas as pd
 from scipy.special import expit
 
 def probability(q, s, xEst, iItem, linear = False):
     vS = np.dot(xEst, iItem) if len(xEst) > 0 else 0
     return q + s + vS if linear else expit(q + s + vS)
 
+def mLogisticD(q, s, xEst, iItem, xPosition, question = False, student = False):
+    probabilityWith = probability(q, s, xEst, iItem, False)
+    xNew = xEst.copy()
+    qN, sN = q, s
+    if question:
+        qN = 0
+    elif student:
+        sN = 0
+    else:
+        xNew[xPosition] = 0
+    probabilityWithout = probability(qN, sN, xNew, iItem, False)
+    return probabilityWith - probabilityWithout
+
 def logisticD(q, s, xEst, iItem, question = False, student = False, xVal = 0):
     vS = np.dot(xEst, iItem) if len(xEst) > 0 else 0
     if question:
         m = q
     elif student:
         m = s
     else:
@@ -37,36 +50,48 @@
 
 def dItemPb(q, s, k, b, xEst, iItem, question = False, student = False, linear = False, xVal = 0):
     if k == 0:
         return probabilityDerivative(q, s, xEst, iItem, question, student, linear, xVal)
     pb = probability(q, s, xEst, iItem, linear)
     return probabilityDerivative(q, s, xEst, iItem, question, student, linear, xVal)*(-1*(1-pb)**(k-1))*(-1*(k+1)*kbcom(k, b)*(-1)*(pb-1)+(k+1)*pb-1)
 
+def makeZero(estX, x, p, size):
+    if size > 0:
+        return estX[x[p]]
+    return 0
+
 def calculateMarginal(position, data, estX, studentSize, questionSize, nCol, linear = False):
     question = True if (position >= studentSize and position < (studentSize + questionSize)) else False
     student = True if position < studentSize else False
     xVarEst = estX[-nCol:] if nCol > 0 else []
-    xVarPos = (studentSize + questionSize) - position - 1 if not (student or question) else 0
+    xVarPos = position - (studentSize + questionSize + nCol) if not (student or question) else 0
     xest = xVarEst[xVarPos] if len(xVarEst) > 0 else 0
     if student or question:
         subData = [x for x in data if position == x[2]] if question else [x for x in data if position == x[1]]
     else:
         subData = [x for x in data if x[xVarPos] != 0]
     minB = min((x[3] for x in subData))
     r = {}
     if not linear:
-        r['Average Logistic'] = [ mean(( probability(estX[x[2]], estX[x[1]], xVarEst, x[-nCol:], linear) for x in subData)) ]
-        r['Average Marginal Logistic'] = [ mean(( logisticD(estX[x[2]], estX[x[1]], xVarEst, x[-nCol:], question, student, xest) for x in subData)) ]
+        r['Average Logistic'] = [ mean(( probability(makeZero(estX, x, 2, questionSize), makeZero(estX, x, 1, studentSize), xVarEst, x[-nCol:], linear) for x in subData)) ]
+        r['Average Marginal Logistic'] = [ mean(( logisticD(makeZero(estX, x, 2, questionSize), makeZero(estX, x, 1, studentSize), xVarEst, x[-nCol:], question, student, xest) for x in subData)) ]
+        r['Average Discrete Marginal Logistic'] = [ mean(( mLogisticD(makeZero(estX, x, 2, questionSize), makeZero(estX, x, 1, studentSize), xVarEst, x[-nCol:], xVarPos, question, student) for x in subData)) ]
     for b in range(0, minB+1):
-        r["ACP k=" + str(b)] = [ mean(( itemPb(estX[x[2]], estX[x[1]], b, minB, xVarEst, x[-nCol:], linear) for x in subData )) ]
+        r["ACP k=" + str(b)] = [ mean(( itemPb(makeZero(estX, x, 2, questionSize), makeZero(estX, x, 1, studentSize), b, minB, xVarEst, x[-nCol:], linear) for x in subData )) ]
     for b in range(0, minB+1):
-        r["AME k=" + str(b)] = [ mean(( dItemPb(estX[x[2]], estX[x[1]], b, minB, xVarEst, x[-nCol:], question, student, linear, xest) for x in subData )) ]
+        r["AME k=" + str(b)] = [ mean(( dItemPb(makeZero(estX, x, 2, questionSize), makeZero(estX, x, 1, studentSize), b, minB, xVarEst, x[-nCol:], question, student, linear, xest) for x in subData )) ]
     return pd.DataFrame(r)
 
 def calculateMarginals(data, estX, studentSize, questionSize, nCol, linear = False):
-    studentResults = pd.concat([ calculateMarginal(x, data, estX, studentSize, questionSize, nCol, linear) for x in range(0, studentSize)], ignore_index=True)
-    rubricResults = pd.concat([ calculateMarginal(x, data, estX, studentSize, questionSize, nCol, linear) for x in range(studentSize, studentSize + questionSize)], ignore_index=True)
+    if studentSize > 0:
+        studentResults = pd.concat([ calculateMarginal(x, data, estX, studentSize, questionSize, nCol, linear) for x in range(0, studentSize)], ignore_index=True)
+    else:
+        studentResults = pd.DataFrame()
+    if questionSize > 0:
+        rubricResults = pd.concat([ calculateMarginal(x, data, estX, studentSize, questionSize, nCol, linear) for x in range(studentSize, studentSize + questionSize)], ignore_index=True)
+    else:
+        rubricResults = pd.DataFrame()
     if nCol > 0:
         varResults = pd.concat([ calculateMarginal(x, data, estX, studentSize, questionSize, nCol, linear) for x in range(studentSize + questionSize, len(estX))], ignore_index=True)
     else:
         varResults = pd.DataFrame()
     return studentResults, rubricResults, varResults
```

### Comparing `ProjectAssessment-0.2.9/ProjectAssessment/Solver.py` & `ProjectAssessment-0.3.0/ProjectAssessment/Solver.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,125 +12,167 @@
 
 @njit
 def kbcom(k, b):
     return -1 if k == b else 0
 
 @njit
 def itemPb2(q, s, k, b, xVari, itemi):
+    if q == 0 and s == 0:
+        return ( np.dot(np.ascontiguousarray(xVari), np.ascontiguousarray(itemi)), k, kbcom(k, b))
+    if q == 0:
+        return ( np.dot(np.ascontiguousarray(xVari), np.ascontiguousarray(itemi)) + s, k, kbcom(k, b))
+    if s == 0:
+        return ( np.dot(np.ascontiguousarray(xVari), np.ascontiguousarray(itemi)) + q, k, kbcom(k, b))
     return ( np.dot(np.ascontiguousarray(xVari), np.ascontiguousarray(itemi)) + q + s, k, kbcom(k, b))
 
 @njit
 def itemPb(q, s, k, b):
     return ( q + s, k, kbcom(k, b))
 
 @njit
-def itemLoop2(x, data, cols = 0):
+def itemLoop2(x, data, cols = 0, no_q = False, no_s = False):
+    if no_q and no_s:
+        return [ itemPb2(0, 0, item[0], item[3], x[-cols:], item[-cols:]) for item in data ]
+    if no_q:
+        return [ itemPb2(0, x[int(item[1])], item[0], item[3], x[-cols:], item[-cols:]) for item in data ]
+    if no_s:
+        return [ itemPb2(x[int(item[2])], 0, item[0], item[3], x[-cols:], item[-cols:]) for item in data ]
     return [ itemPb2(x[int(item[2])], x[int(item[1])], item[0], item[3], x[-cols:], item[-cols:]) for item in data ]
 
 @njit
 def itemLoop(x, data):
     return [ itemPb(x[int(item[2])], x[int(item[1])], item[0], item[3]) for item in data ]
 
 @njit
 def itemLoopRestricted(x, data):
     return [ ( x[0], item[0], kbcom(item[0], item[3])) for item in data ]
 
-def opFunction(x, data, linear = False, cols = 0):
+def opFunction(x, data, linear = False, cols = 0, no_q = False, no_s = False):
     if cols > 0:
-        dem = np.array(itemLoop2(x, data, cols))
+        dem = np.array(itemLoop2(x, data, cols, no_q, no_s))
     else:
         dem = np.array(itemLoop(x, data))
     vS = dem[:,0] if linear else expit(dem[:,0])
-    return -1.0 * np.sum(xlogy(1,  vS + (vS - 1) * dem[:,2]) + xlog1py(dem[:,1], -vS))
+    return -np.sum(xlogy(1,  vS + (vS - 1) * dem[:,2]) + xlog1py(dem[:,1], -vS))
 
 def opRestricted (x, data, linear = False):
     dem = np.array(itemLoopRestricted(x, data))
     vS = dem[:,0] if linear else expit(dem[:,0])
-    return -1.0 * np.sum(xlogy(1,  vS + (vS - 1) * dem[:,2]) + xlog1py(dem[:,1], -vS))
+    return -np.sum(xlogy(1,  vS + (vS - 1) * dem[:,2]) + xlog1py(dem[:,1], -vS))
 
-def solve(dataset, summary = True, linear = False, columns = None):
+def solve(dataset, summary = True, linear = False, columns = None, no_q = False, no_s = False):
     studentCode, uniqueStudents = pd.factorize(dataset['student'])
     questionCode, uniqueQuestion = pd.factorize(dataset['rubric'])
-    questionCode = questionCode + uniqueStudents.size
-    smap = np.concatenate((uniqueStudents, uniqueQuestion), axis=None).tolist()
+    if no_q and no_s:
+        smap = []
+    elif no_q:
+        smap = uniqueStudents.tolist()
+    elif no_s:
+        smap = uniqueQuestion.tolist()
+    else:
+        questionCode = questionCode + uniqueStudents.size
+        smap = np.concatenate((uniqueStudents, uniqueQuestion), axis=None).tolist()
     data = list(zip(dataset['k'].to_numpy().flatten().tolist(), studentCode.tolist(), questionCode.tolist(), dataset['bound'].to_numpy().flatten().tolist()))
     for i, _ in enumerate(data):
         for col in columns:
             data[i] = data[i] + (dataset[col].iloc[i],)
     if linear:
-        bounds = ((0, 1),) * (uniqueStudents.size + uniqueQuestion.size + len(columns))
+        if no_q and no_s:
+            bounds = ((0, 1),) * len(columns)
+        elif no_q:
+            bounds = ((0, 1),) * (uniqueStudents.size + len(columns))
+        elif no_s:
+            bounds = ((0, 1),) * (uniqueQuestion.size + len(columns))
+        else:
+            bounds = ((0, 1),) * (uniqueStudents.size + uniqueQuestion.size + len(columns))
     else:
         bounds = None
-    minValue = minimize(opFunction, np.array((1/(2*(1+dataset['k'].mean())),)*(len(smap) + len(columns)), np.dtype(float)), args=(np.array(data, np.dtype(float)), linear, len(columns)), method='Powell', bounds=bounds)
+    minValue = minimize(opFunction, np.array((1/(2*(1+dataset['k'].mean())),)*(len(smap) + len(columns)), np.dtype(float)), args=(np.array(data, np.dtype(float)), linear, len(columns), no_q, no_s), method='Powell', bounds=bounds)
     if minValue.success:
         estX = minValue.x.flatten().tolist()
         varNames = smap + columns
         fullResults = list(zip(varNames, estX))
         cols = ['Variable', 'Value']
-        studentResults = pd.DataFrame(fullResults[:uniqueStudents.size], columns=cols)
-        questionResults = pd.DataFrame(fullResults[uniqueStudents.size:len(smap)], columns=cols)
-        varResults = pd.DataFrame(fullResults[len(smap):], columns=cols)
+        if no_q and no_s:
+            studentResults = pd.DataFrame(columns=cols)
+            questionResults = pd.DataFrame(columns=cols)
+            varResults = pd.DataFrame(fullResults, columns=cols)
+        elif no_q:
+            studentResults = pd.DataFrame(fullResults[:uniqueStudents.size], columns=cols)
+            questionResults = pd.DataFrame(columns=cols)
+            varResults = pd.DataFrame(fullResults[uniqueStudents.size:], columns=cols)
+        elif no_s:
+            studentResults = pd.DataFrame(columns=cols)
+            questionResults = pd.DataFrame(fullResults[:uniqueQuestion.size], columns=cols)
+            varResults = pd.DataFrame(fullResults[uniqueQuestion.size:], columns=cols)
+        else:
+            studentResults = pd.DataFrame(fullResults[:uniqueStudents.size], columns=cols)
+            questionResults = pd.DataFrame(fullResults[uniqueStudents.size:len(smap)], columns=cols)
+            varResults = pd.DataFrame(fullResults[len(smap):], columns=cols)
         if not summary:
             return {
                 'student': studentResults,
                 'rubric': questionResults,
                 'variables': varResults
             }
-        studentMarginals, rubricMarginals, varMarginals = calculateMarginals(data, estX, uniqueStudents.size, uniqueQuestion.size, len(columns), linear)
+        parStudents, parQuestion, parVar = (len(studentResults.index), len(questionResults.index), len(varResults.index))
+        studentMarginals, rubricMarginals, varMarginals = calculateMarginals(data, estX, parStudents, parQuestion, parVar, linear)
         d = {
             'student': studentResults.join(studentMarginals),
             'rubric': questionResults.join(rubricMarginals),
             'variables': varResults.join(varMarginals)
         }
         d['LogLikelihood'] = -1.0 * minValue.fun
-        d['AIC'] = 2*(uniqueStudents.size+uniqueQuestion.size+len(columns))+2*minValue.fun
-        d['BIC'] = (uniqueStudents.size+uniqueQuestion.size+len(columns))*np.log(len(studentCode))+2*minValue.fun
+        d['AIC'] = 2*(parStudents + parQuestion + parVar)+2*minValue.fun
+        d['BIC'] = (parStudents + parQuestion + parVar)*np.log(len(studentCode))+2*minValue.fun
         d['n'] = len(studentCode)
-        d['NumberOfParameters'] = uniqueStudents.size+uniqueQuestion.size+len(columns)
+        d['NumberOfParameters'] = parStudents + parQuestion + parVar
         if linear:
             boundsSingle = ((0, 1),)
         else:
             boundsSingle = None
         minRestricted = minimize(opRestricted, np.array((1/(1+dataset['k'].mean()),), np.dtype(float)), args=(np.array(data, np.dtype(float)), linear), method='Powell', bounds=boundsSingle)
         if minRestricted.success:
             d['McFadden'] = 1 - minValue.fun/minRestricted.fun
             d['LR'] = -2*(-1*minRestricted.fun+minValue.fun)
-            d['Chi-Squared'] = chi2.sf(d['LR'], (uniqueStudents.size+uniqueQuestion.size+len(columns)-1))
+            d['Chi-Squared'] = chi2.sf(d['LR'], (parStudents + parQuestion + parVar - 1))
         return d
     if not summary:
         return None
     raise Exception(minValue.message)
 
-def bootstrapRow (dataset, columns, rubric=False, linear=False):
+def bootstrapRow (dataset, columns, rubric=False, linear=False, no_q = False, no_s = False):
     key = 'rubric' if rubric else 'student'
     ids = dataset[key].unique().flatten().tolist()
     randomGroupIds = np.random.choice(ids, size=len(ids), replace=True)
     l = []
     for c, i in enumerate(randomGroupIds):
         rows = dataset[dataset[key]==i]
         rows = rows.assign(rubric=c) if rubric else rows.assign(student=c)
         l.append(rows)
     resultData = pd.concat(l, ignore_index=True)
-    return solve(resultData, False, linear, columns)
+    return solve(resultData, False, linear, columns, no_q, no_s)
 
 def CallRow(row):
     key = 'student' if row['rubric'] else 'rubric'
-    r = bootstrapRow(row['dataset'], row['columns'], row['rubric'], row['linear'])
+    r = bootstrapRow(row['dataset'], row['columns'], row['rubric'], row['linear'], row['no_q'], row['no_s'])
     if r is not None:
         return (r[key], r['variables'])
     return None
 
-def bootstrap(dataset, n, rubric=False, linear=False, columns=None):
+def bootstrap(dataset, n, rubric=False, linear=False, columns=None, no_q = False, no_s = False):
     l = []
     rows = [
         {
             'dataset': dataset,
             'rubric': rubric,
             'linear': linear,
-            'columns': columns
+            'columns': columns,
+            'no_q': no_q,
+            'no_s': no_s
         }
     ]*n
     p = Pool()
     nones = []
     for _, result in tqdm(enumerate(p.imap_unordered(CallRow, rows)), total=n):
         if result is not None:
             keyresult, varresult = result
@@ -144,32 +186,36 @@
         'results': pd.concat(l, ignore_index=True),
         'nones': len(nones)
     }
 
 def compareKBound(x):
     return pd.to_numeric(x, downcast='integer')
 
-def getResults(dataset: pd.DataFrame,c=0.025, rubric=False, n=1000, linear=False, columns=None):
+def getResults(dataset: pd.DataFrame,c=0.025, rubric=False, n=1000, linear=False, columns=None, no_students=False, no_questions=False):
     """
     Estimates the parameters of the model and produces confidence intervals for the estimates using a bootstrap method.
 
     Parameters:
     -----------
     dataset : Pandas DataFrame
-        A dataframe with the following columns: k, student, rubric, bound.  Student and rubric identifiers for the student and rubric items.  Bound is maximum bin in the rubric that can be reached.  k is the bin the bin the student reached on a given rubric item.
+        A dataframe with the following columns: k, student, rubric, bound.  Student and rubric identifiers for the student and rubric items.  Bound is maximum bin in the rubric that can be reached.  k is the bin the student reached on a given rubric item.
     c : float
         Confidence level for the confidence intervals.  Defaults to 0.025.
     rubric : bool
         Switches the bootstrap to treating the rubric rows as blocks instead of the students.  Defaults to False.
     n : int
         Number of iterations for the bootstrap.  Defaults to 1000.
-    linear: bool
+    linear : bool
         Uses a simple linear combination of the rubric and student items instead of a sigmoid function.  Defaults to False.
-    columns: list
+    columns : list
         A list of column names to include in the model.  The column names cannot be in common with any of the rubric row identifiers.  Defaults to None.
+    no_students : bool
+        If True, the model will not include student (s_i) estimates.  Defaults to False.
+    no_questions : bool
+        If True, the model will not include question/rubric row (q_j) estimates.  Defaults to False.
 
     Returns:
         Tuple:
             Rubric and Arbitrary Column Estimates : Pandas DataFrame
             Student Estimates : Pandas DataFrame
             Bootstrap CIs and P-Values : Pandas DataFrame
             # of Times no solution could be found in the Bootstrap : int
@@ -198,18 +244,30 @@
     if len(columns) > 0 and not set(columns).issubset(dataset.columns):
         raise Exception('Specified columns not in dataset')
     dataset.dropna(inplace=True)
     dataset = dataset[pd.to_numeric(dataset['k'], errors='coerce').notnull()]
     dataset = dataset[pd.to_numeric(dataset['bound'], errors='coerce').notnull()]
     dataset[["k", "bound"]] = dataset[["k", "bound"]].apply(compareKBound)
     dataset = dataset[dataset['k'] <= dataset['bound']]
+    no_s = False
+    no_q = False
+    if len(columns) > 0:
+        for spec in columns:
+            dataset = dataset[pd.to_numeric(dataset[spec], errors='coerce').notnull()]
+        dataset[columns] = dataset[columns].apply(pd.to_numeric)
+        if set(columns).intersection(set(dataset['rubric'].unique())):
+            raise Exception('Specified columns cannot be in common with any of the rubric row identifiers.')
+        if no_students:
+            no_s = True
+        if no_questions:
+            no_q = True
     if not len(dataset.index) > 0:
         raise Exception('Invalid pandas dataset, empty dataset.')
     print("Estimating Parameters ...")
-    estimates = solve(dataset, linear=linear, columns=columns)
+    estimates = solve(dataset, linear=linear, columns=columns, no_q=no_q, no_s=no_s)
     print("... Done. Bootstrapping ...")
     if estimates is not None:
         results = bootstrap(dataset, n, rubric, linear=linear, columns=columns)
         r = results['results']
         l = []
         for var in r['Variable'].unique():
             df = r[r['Variable'] == var]['Value']
@@ -230,32 +288,36 @@
             LR = estimates["LR"]
             ChiSquared = estimates["Chi-Squared"]
         combined = pd.concat([estimates['rubric'], estimates['variables']], ignore_index=True)
         return (combined, estimates['student'], pd.DataFrame(l), results['nones'], estimates['n'], estimates['NumberOfParameters'], estimates['AIC'], estimates['BIC'], McFadden, LR, ChiSquared, estimates['LogLikelihood'])
     else:
         raise Exception('Could not find estimates.')
 
-def DisplayResults(dataset: pd.DataFrame,c=0.025, rubric=False, n=1000, linear=False, columns=None):
+def DisplayResults(dataset: pd.DataFrame,c=0.025, rubric=False, n=1000, linear=False, columns=None, no_students=False, no_questions=False):
     """
     Estimates the parameters of the model and produces confidence intervals for the estimates using a bootstrap method. Results are printed out to the console.
 
     Parameters:
     -----------
     dataset : Pandas DataFrame
-        A dataframe with the following columns: k, student, rubric, bound.  Student and rubric identifiers for the student and rubric items.  Bound is maximum bin in the rubric that can be reached.  k is the bin the bin the student reached on a given rubric item.
+        A dataframe with the following columns: k, student, rubric, bound.  Student and rubric identifiers for the student and rubric items.  Bound is maximum bin in the rubric that can be reached.  k is the bin the student reached on a given rubric item.
     c : float
         Confidence level for the confidence intervals.  Defaults to 0.025.
     rubric : bool
         Switches the bootstrap to treating the rubric rows as blocks instead of the students.  Defaults to False.
     n : int
         Number of iterations for the bootstrap.  Defaults to 1000.
-    linear: bool
+    linear : bool
         Uses a simple linear combination of the rubric and student items instead of a sigmoid function.  Defaults to False.
-    columns: list
+    columns : list
         A list of column names to include in the model. The column names cannot be in common with any of the rubric row identifiers. Defaults to None.
+    no_students : bool
+        If True, the model will not include student (s_i) estimates.  Defaults to False.
+    no_questions : bool
+        If True, the model will not include question/rubric row (q_j) estimates.  Defaults to False.
 
     Returns:
         Tuple:
             Rubric and Arbitrary Column Estimates : Pandas DataFrame
             Student Estimates : Pandas DataFrame
             Bootstrap CIs and P-Values : Pandas DataFrame
             # of Times no solution could be found in the Bootstrap : int
@@ -265,15 +327,15 @@
             BIC : float
             McFadden R^2 : float
             Likelihood Ratio Test Statistic of the model : float
             Chi-Squared P-Value of the model : float
             Log Likelihood : float
 
     """
-    rubricR, studentR, bootstrapR, countE, obs, param, AIC, BIC, McFadden, LR, ChiSquared, LogLikelihood = getResults(dataset, c, rubric, n, linear, columns=columns)
+    rubricR, studentR, bootstrapR, countE, obs, param, AIC, BIC, McFadden, LR, ChiSquared, LogLikelihood = getResults(dataset, c, rubric, n, linear, columns=columns, no_students=no_students, no_questions=no_questions)
     warnings = []
     if rubric is True:
         printedStudent = studentR.merge(bootstrapR, on='Variable', how='left')
         if isinstance(columns, list) and len(columns) > 0:
             specialbootstrap = bootstrapR[bootstrapR['Variable'].isin(columns)]
             printedRubric = rubricR.merge(specialbootstrap, on='Variable', how='left')
         else:
@@ -307,38 +369,42 @@
     MakeTwoByTwoTable(x)
     if len(warnings) > 0:
         print('Warnings:')
         for warning in warnings:
             print(warning)
     return (rubricR, studentR, bootstrapR, countE, obs, param, AIC, BIC, McFadden, LR, ChiSquared, LogLikelihood)
 
-def SaveResults(dataset: pd.DataFrame,c=0.025, rubric=False, n=1000, linear=False, rubricFile = 'rubric.csv', studentFile = 'student.csv', outputFile = 'output.csv', columns=None):
+def SaveResults(dataset: pd.DataFrame,c=0.025, rubric=False, n=1000, linear=False, rubricFile = 'rubric.csv', studentFile = 'student.csv', outputFile = 'output.csv', columns=None, no_students=False, no_questions=False):
     """
     Estimates the parameters of the model and produces confidence intervals for the estimates using a bootstrap method. Results are printed out to the console and saved to CSV files.
 
     Parameters:
     -----------
     dataset : Pandas DataFrame
-        A dataframe with the following columns: k, student, rubric, bound.  Student and rubric identifiers for the student and rubric items.  Bound is maximum bin in the rubric that can be reached.  k is the bin the bin the student reached on a given rubric item.
+        A dataframe with the following columns: k, student, rubric, bound.  Student and rubric identifiers for the student and rubric items.  Bound is maximum bin in the rubric that can be reached.  k is the bin the student reached on a given rubric item.
     c : float
         Confidence level for the confidence intervals.  Defaults to 0.025.
     rubric : bool
         Switches the bootstrap to treating the rubric rows as blocks instead of the students.  Defaults to False.
     n : int
         Number of iterations for the bootstrap.  Defaults to 1000.
     linear: bool
         Uses a simple linear combination of the rubric and student items instead of a sigmoid function.  Defaults to False.
     rubricFile : str
         File name/path for the rubric results.  Defaults to 'rubric.csv'.
     studentFile : str
         File name/path for the student results.  Defaults to 'student.csv'.
     outputFile : str
         File name/path for the summary output results.  Defaults to 'output.csv'.
-    columns: list
+    columns : list
         A list of column names to include in the model. The column names cannot be in common with any of the rubric row identifiers. Defaults to None.
+    no_students : bool
+        If True, the model will not include student (s_i) estimates.  Defaults to False.
+    no_questions : bool
+        If True, the model will not include question/rubric row (q_j) estimates.  Defaults to False.
 
     Returns:
         Tuple:
             Rubric and Arbitrary Column Estimates : Pandas DataFrame
             Student Estimates : Pandas DataFrame
             Bootstrap CIs and P-Values : Pandas DataFrame
             # of Times no solution could be found in the Bootstrap : int
@@ -348,15 +414,15 @@
             BIC : float
             McFadden R^2 : float
             Likelihood Ratio Test Statistic of the model : float
             Chi-Squared P-Value of the model : float
             Log Likelihood : float
 
     """
-    rubricR, studentR, bootstrapR, countE, obs, param, AIC, BIC, McFadden, LR, ChiSquared, LogLikelihood  = DisplayResults(dataset, c, rubric, n, linear, columns=columns)
+    rubricR, studentR, bootstrapR, countE, obs, param, AIC, BIC, McFadden, LR, ChiSquared, LogLikelihood  = DisplayResults(dataset, c, rubric, n, linear, columns=columns, no_students=no_students, no_questions=no_questions)
 
     if rubric is True:
         printedStudent = studentR.merge(bootstrapR, on='Variable', how='left')
         if isinstance(columns, list) and len(columns) > 0:
             specialbootstrap = bootstrapR[bootstrapR['Variable'].isin(columns)]
             printedRubric = rubricR.merge(specialbootstrap, on='Variable', how='left')
         else:
```

### Comparing `ProjectAssessment-0.2.9/ProjectAssessment.egg-info/PKG-INFO` & `ProjectAssessment-0.3.0/ProjectAssessment.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: ProjectAssessment
-Version: 0.2.9
+Version: 0.3.0
 Summary: Package to compute the Project-Based Assessment estimates of student and rubric proficiency.
 Home-page: https://github.com/tazzben/project-based-assessment
-Download-URL: https://github.com/tazzben/project-based-assessment/archive/v0.2.9.tar.gz
+Download-URL: https://github.com/tazzben/project-based-assessment/archive/v0.3.0.tar.gz
 Author: Ben Smith
 Author-email: bosmith@unomaha.edu
 License: MIT
 Keywords: Assessment,Projects,Statistics,Education,Bootstrap
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ProjectAssessment-0.2.9/README.md` & `ProjectAssessment-0.3.0/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -6,21 +6,28 @@
 
 * getResults
 * DisplayResults
 * SaveResults
 
 getResults and DisplayResults take the following parameters: 
 
-1. A pandas Dataset containing the columns "k", "student", "rubric", "bound".  The "k" column is the rubric level the given student reached on the given rubric row. The "student" column is a student identifier. The "rubric" column is a rubric row identifier. The "bound" column is maximum "k" value possible on the given rubric row.
-2. A float between 0 and 0.5 indicating the portion of the bootstrapped EDF to extract.  For instance, specifying 0.025 would produce the 95% confidence interval. Default is 0.025.
-3. A bool flag indicating to treat the rubric rows as blocks instead of the unique students in the bootstrap.  Defaults to False.
-4. The number of iterations in the bootstrap.  Defaults to 1000.
-5. Uses a simple linear combination of the rubric and student items instead of a sigmoid function when set to true.  Defaults to False.
-
-SaveResults takes the same parameters as getResults and DisplayResults but has the additional parameters of: rubricFile, studentFile, and outputFile (in that order).  These specify the filenames to save the results.  These default to "rubric.csv", "student.csv", and "output.csv".
+1. dataset: A pandas Dataset containing the columns "k", "student", "rubric", "bound".  The "k" column is the rubric level the given student reached on the given rubric row. The "student" column is a student identifier. The "rubric" column is a rubric row identifier. The "bound" column is maximum "k" value possible on the given rubric row.
+2. c: A float between 0 and 0.5 indicating the portion of the bootstrapped EDF to extract.  For instance, specifying 0.025 would produce the 95% confidence interval. Default is 0.025.
+3. rubric: A bool flag indicating to treat the rubric rows as blocks instead of the unique students in the bootstrap.  Defaults to False.
+4. n: The number of iterations in the bootstrap.  Defaults to 1000.
+5. linear: Uses a simple linear combination of the rubric and student items instead of a sigmoid function when set to true.  Defaults to False.
+6. columns: A list of column names to include in the model. The column names cannot be in common with any of the rubric row identifiers. Defaults to None.
+7. no_students: If True, the model will not include student (s_i) estimates.  Defaults to False.
+8. no_questions: If True, the model will not include question/rubric row (q_j) estimates.  Defaults to False.
+
+SaveResults includes the same parameters as getResults and DisplayResults but has three additional parameters: 
+
+1. rubricFile: File name/path for the rubric results.  Defaults to 'rubric.csv'.
+2. studentFile: File name/path for the student results.  Defaults to 'student.csv'.
+3. outputFile: File name/path for the summary output results.  Defaults to 'output.csv'.
 
 All methods return the following:
 
 1. Rubric difficulty estimates as a pandas dataframe. Additional interpretation columns are provided in this dataframe that will be described below.
 2. Student ability estimates as a pandas dataframe.  Additional interpretation columns are provided in this dataframe that will be described below.
 3. Bootstrap confidence intervals and P-Values as a pandas dataframe. P-Values are only provided when estimating the non-linear model as they will always be zero for the linear model (by construction the estimates are constrained between 0 and 1 in the linear model).
 4. The number of times the bootstrap routine could not find a solution (if any).
@@ -36,15 +43,16 @@
 getResults only return these values as a tuple.  DisplayResults returns the values as a tuple and prints the results to screen.  SaveResults returns the values as a tuple, displays the results and saves the results to CSV files.
 
 The rubric difficulty and student ability pandas dataframes return estimates along with columns used for interpretation.  The following columns are provided: 
 
 * AME k=i: The average marginal effect of k=i.  This is provided for all possible bins (i between 0 and the highest bin).  This procedure calculates the marginal effect for a given estimate conditioned on k=i for all observations impacted by the estimate.  The average is then calculated. These values will sum to zero.
 * ACP k=i: While average marginal effect is the standard approach to interpreting MLE results (especially in a logit or probit context), we don't think they are particularly useful in this model.  Therefore, the application also provides columns for the average conditional probability of k=i.  Given the subset of the data used to calculate AME, this is the average probability of k=i given the estimated value.  When the dataset is balanced (all students have a score for all rubric rows), these values will sum to 1.  Note that the top bin is capturing the censoring effect. Therefore, it is common that a substantial probability is estimated for this bin.
 * Average Logistic: This estimate is only provided when estimating the non-linear model.  It is the average of the probability function given the estimated value.  It uses the same subset of the data used to calculate AME and ACP above.  In terms of interpretation, it is the average probability of failure to proceed to the next bin.  Therefore, it will equal ACP k=0.
-* Average Marginal Logistic: This estimate is only provided when estimating the non-linear model.  It is the average of the marginal probability function given the estimated value.  It uses the same subset of the data used to calculate AME and ACP above.  In terms of interpretation, it is the change in the average probability of failure to proceed to the next bin.
+* Average Marginal Logistic: This estimate is only provided when estimating the non-linear model.  It is the average of the marginal probability function (derivative) given the estimated value.  It uses the same subset of the data used to calculate AME and ACP above.  In terms of interpretation, it is the change in the average probability of failure to proceed to the next bin.
+* Average Discrete Marginal Logistic: This estimate is only provided when estimating the non-linear model.  It is the average of the discrete marginal probability function given the estimated value.  It uses the same subset of the data used to calculate AME and ACP above.  In terms of interpretation, it is the change in the average probability of failure to proceed to the next bin.  This is very similar to the Average Marginal Logistic above and will often produce very similar values.  However, this value is calculated by calculating the probability with the variable in question and without the variable in question and then taking the difference.  This is a common approach when calculating the discrete marginal effect in logit and probit models.  The Average Marginal Logistic is calculated by taking the derivative. Where these values tend to diverge is when the estimate is at an extreme.  Consider a student who has extremely low ability such that they fail every trial.  In this case, the derivative will be near zero as it is the instantaneous slope at the extreme value.  However, the Discrete Marginal Logistic will be very large as the average change in probability over the range is large.  
 
 ## Background and Use
 
 This package is based on the estimator presented in "[Assessing Proxies of Knowledge and Difficulty with Rubric-Based Instruments](https://dx.doi.org/10.2139/ssrn.4194935)."  There is a [video](https://vimeo.com/735183858) demonstrating using this package in Google Colab and a [video](https://vimeo.com/756447388) explaining the paper.   
 
 ## Installation
```

### Comparing `ProjectAssessment-0.2.9/setup.py` & `ProjectAssessment-0.3.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from distutils.core import setup
 
 setup(
     name='ProjectAssessment',
-    version='0.2.9',
+    version='0.3.0',
     packages=['ProjectAssessment',],
     python_requires='>3.7.0',
     license='MIT',
     install_requires=[
         'numpy>=1.21.0',
         'pandas>=1.3.0',
         'tqdm',
@@ -22,10 +22,10 @@
     'Programming Language :: Python :: 3.10',
     'Programming Language :: Python :: 3.9',
     'Programming Language :: Python :: 3.8',
     'Programming Language :: Python :: 3.7',
     ],
     keywords = ['Assessment', 'Projects', 'Statistics', 'Education', 'Bootstrap'],
     url = 'https://github.com/tazzben/project-based-assessment',
-    download_url = 'https://github.com/tazzben/project-based-assessment/archive/v0.2.9.tar.gz',
+    download_url = 'https://github.com/tazzben/project-based-assessment/archive/v0.3.0.tar.gz',
     description = 'Package to compute the Project-Based Assessment estimates of student and rubric proficiency.',
 )
```

