# Comparing `tmp/data-science-toolkit-0.0.999.tar.gz` & `tmp/data-science-toolkit-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "E:\projects\dst\dist\tmpzj8mfama\data-science-toolkit-0.0.999.tar", last modified: Sat May 13 00:45:18 2023, max compression
+gzip compressed data, was "E:\projects\dst\dist\tmps7rcvnnq\data-science-toolkit-0.1.0.tar", last modified: Sat May 13 01:01:17 2023, max compression
```

## Comparing `data-science-toolkit-0.0.999.tar` & `data-science-toolkit-0.1.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-05-13 00:45:18.000000 data-science-toolkit-0.0.999/
--rw-rw-rw-   0        0        0     1096 2022-03-25 12:00:42.000000 data-science-toolkit-0.0.999/LICENSE
--rw-rw-rw-   0        0        0     1965 2023-05-13 00:45:18.000000 data-science-toolkit-0.0.999/PKG-INFO
--rw-rw-rw-   0        0        0     1355 2022-04-14 01:06:21.000000 data-science-toolkit-0.0.999/README.md
--rw-rw-rw-   0        0        0      387 2022-03-25 12:00:42.000000 data-science-toolkit-0.0.999/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-13 00:45:18.000000 data-science-toolkit-0.0.999/setup.cfg
--rw-rw-rw-   0        0        0     1435 2023-05-13 00:44:55.000000 data-science-toolkit-0.0.999/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-13 00:45:17.000000 data-science-toolkit-0.0.999/src/
-drwxrwxrwx   0        0        0        0 2023-05-13 00:45:18.000000 data-science-toolkit-0.0.999/src/data_science_toolkit/
--rw-rw-rw-   0        0        0        0 2022-03-25 12:00:42.000000 data-science-toolkit-0.0.999/src/data_science_toolkit/__init__.py
--rw-rw-rw-   0        0        0    10268 2022-03-25 12:00:42.000000 data-science-toolkit-0.0.999/src/data_science_toolkit/chart.py
--rw-rw-rw-   0        0        0     6375 2022-05-20 00:30:43.000000 data-science-toolkit-0.0.999/src/data_science_toolkit/csm.py
--rw-rw-rw-   0        0        0    70325 2023-05-12 20:58:24.000000 data-science-toolkit-0.0.999/src/data_science_toolkit/dataframe.py
--rw-rw-rw-   0        0        0    12467 2022-05-20 00:36:43.000000 data-science-toolkit-0.0.999/src/data_science_toolkit/gis.py
--rw-rw-rw-   0        0        0     8456 2022-03-25 12:00:42.000000 data-science-toolkit-0.0.999/src/data_science_toolkit/imagefactory.py
--rw-rw-rw-   0        0        0    25115 2023-05-13 00:40:51.000000 data-science-toolkit-0.0.999/src/data_science_toolkit/lib.py
--rw-rw-rw-   0        0        0    28669 2023-03-15 23:27:50.000000 data-science-toolkit-0.0.999/src/data_science_toolkit/model.py
--rw-rw-rw-   0        0        0     7636 2022-05-20 00:33:21.000000 data-science-toolkit-0.0.999/src/data_science_toolkit/r3.py
--rw-rw-rw-   0        0        0     4983 2021-02-01 01:53:23.000000 data-science-toolkit-0.0.999/src/data_science_toolkit/rl.py
--rw-rw-rw-   0        0        0     1445 2022-05-19 23:54:12.000000 data-science-toolkit-0.0.999/src/data_science_toolkit/rl_dqn.py
--rw-rw-rw-   0        0        0     5488 2023-03-15 23:28:40.000000 data-science-toolkit-0.0.999/src/data_science_toolkit/vectorizer.py
-drwxrwxrwx   0        0        0        0 2023-05-13 00:45:18.000000 data-science-toolkit-0.0.999/src/data_science_toolkit.egg-info/
--rw-rw-rw-   0        0        0     1965 2023-05-13 00:45:13.000000 data-science-toolkit-0.0.999/src/data_science_toolkit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      709 2023-05-13 00:45:15.000000 data-science-toolkit-0.0.999/src/data_science_toolkit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-13 00:45:13.000000 data-science-toolkit-0.0.999/src/data_science_toolkit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      209 2023-05-13 00:45:14.000000 data-science-toolkit-0.0.999/src/data_science_toolkit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-05-13 00:45:14.000000 data-science-toolkit-0.0.999/src/data_science_toolkit.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-13 00:45:18.000000 data-science-toolkit-0.0.999/test/
--rw-rw-rw-   0        0        0       85 2022-03-25 12:00:42.000000 data-science-toolkit-0.0.999/test/test.py
+drwxrwxrwx   0        0        0        0 2023-05-13 01:01:17.000000 data-science-toolkit-0.1.0/
+-rw-rw-rw-   0        0        0     1096 2022-03-25 12:00:42.000000 data-science-toolkit-0.1.0/LICENSE
+-rw-rw-rw-   0        0        0     1963 2023-05-13 01:01:17.000000 data-science-toolkit-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1355 2022-04-14 01:06:21.000000 data-science-toolkit-0.1.0/README.md
+-rw-rw-rw-   0        0        0      387 2022-03-25 12:00:42.000000 data-science-toolkit-0.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-13 01:01:17.000000 data-science-toolkit-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1433 2023-05-13 01:00:53.000000 data-science-toolkit-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-13 01:01:17.000000 data-science-toolkit-0.1.0/src/
+drwxrwxrwx   0        0        0        0 2023-05-13 01:01:17.000000 data-science-toolkit-0.1.0/src/data_science_toolkit/
+-rw-rw-rw-   0        0        0        0 2022-03-25 12:00:42.000000 data-science-toolkit-0.1.0/src/data_science_toolkit/__init__.py
+-rw-rw-rw-   0        0        0    10268 2022-03-25 12:00:42.000000 data-science-toolkit-0.1.0/src/data_science_toolkit/chart.py
+-rw-rw-rw-   0        0        0     6375 2022-05-20 00:30:43.000000 data-science-toolkit-0.1.0/src/data_science_toolkit/csm.py
+-rw-rw-rw-   0        0        0    74392 2023-05-13 01:00:41.000000 data-science-toolkit-0.1.0/src/data_science_toolkit/dataframe.py
+-rw-rw-rw-   0        0        0    12467 2022-05-20 00:36:43.000000 data-science-toolkit-0.1.0/src/data_science_toolkit/gis.py
+-rw-rw-rw-   0        0        0     8456 2022-03-25 12:00:42.000000 data-science-toolkit-0.1.0/src/data_science_toolkit/imagefactory.py
+-rw-rw-rw-   0        0        0    25115 2023-05-13 00:40:51.000000 data-science-toolkit-0.1.0/src/data_science_toolkit/lib.py
+-rw-rw-rw-   0        0        0    28669 2023-03-15 23:27:50.000000 data-science-toolkit-0.1.0/src/data_science_toolkit/model.py
+-rw-rw-rw-   0        0        0     7636 2022-05-20 00:33:21.000000 data-science-toolkit-0.1.0/src/data_science_toolkit/r3.py
+-rw-rw-rw-   0        0        0     4983 2021-02-01 01:53:23.000000 data-science-toolkit-0.1.0/src/data_science_toolkit/rl.py
+-rw-rw-rw-   0        0        0     1445 2022-05-19 23:54:12.000000 data-science-toolkit-0.1.0/src/data_science_toolkit/rl_dqn.py
+-rw-rw-rw-   0        0        0     5488 2023-03-15 23:28:40.000000 data-science-toolkit-0.1.0/src/data_science_toolkit/vectorizer.py
+drwxrwxrwx   0        0        0        0 2023-05-13 01:01:17.000000 data-science-toolkit-0.1.0/src/data_science_toolkit.egg-info/
+-rw-rw-rw-   0        0        0     1963 2023-05-13 01:01:14.000000 data-science-toolkit-0.1.0/src/data_science_toolkit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      709 2023-05-13 01:01:15.000000 data-science-toolkit-0.1.0/src/data_science_toolkit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-13 01:01:14.000000 data-science-toolkit-0.1.0/src/data_science_toolkit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      209 2023-05-13 01:01:15.000000 data-science-toolkit-0.1.0/src/data_science_toolkit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-05-13 01:01:15.000000 data-science-toolkit-0.1.0/src/data_science_toolkit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-13 01:01:17.000000 data-science-toolkit-0.1.0/test/
+-rw-rw-rw-   0        0        0       85 2022-03-25 12:00:42.000000 data-science-toolkit-0.1.0/test/test.py
```

### Comparing `data-science-toolkit-0.0.999/LICENSE` & `data-science-toolkit-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `data-science-toolkit-0.0.999/PKG-INFO` & `data-science-toolkit-0.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data-science-toolkit
-Version: 0.0.999
+Version: 0.1.0
 Summary: Data Science Toolkit (DST) is a Python library that helps implement data science related project with ease.
 Home-page: https://github.com/elhachimi-ch/dst
 Author: EL HACHIMI CHOUAIB
 Author-email: elhachimi.ch@gmail.com
 Project-URL: Bug Tracker, https://github.com/elhachimi-ch/dst/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `data-science-toolkit-0.0.999/README.md` & `data-science-toolkit-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `data-science-toolkit-0.0.999/setup.py` & `data-science-toolkit-0.1.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
     
     
 setuptools.setup(
     name="data-science-toolkit",
-    version="0.0.999",
+    version="0.1.0",
     author="EL HACHIMI CHOUAIB",
     author_email="elhachimi.ch@gmail.com",
     description="Data Science Toolkit (DST) is a Python library that helps implement data science related project with ease.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/elhachimi-ch/dst",
     project_urls={
```

### Comparing `data-science-toolkit-0.0.999/src/data_science_toolkit/chart.py` & `data-science-toolkit-0.1.0/src/data_science_toolkit/chart.py`

 * *Files identical despite different names*

### Comparing `data-science-toolkit-0.0.999/src/data_science_toolkit/csm.py` & `data-science-toolkit-0.1.0/src/data_science_toolkit/csm.py`

 * *Files identical despite different names*

### Comparing `data-science-toolkit-0.0.999/src/data_science_toolkit/dataframe.py` & `data-science-toolkit-0.1.0/src/data_science_toolkit/dataframe.py`

 * *Files 13% similar despite different names*

```diff
@@ -17,95 +17,96 @@
 from sklearn.datasets import load_iris
 from collections import Counter
 from .chart import Chart
 import numpy as np
 import nltk
 from nltk.tokenize import sent_tokenize, word_tokenize
 
+
 class DataFrame:
     """
     """
     __vectorizer = None
     __generator = None
 
     def __init__(self, data_link=None, columns_names_as_list=None, data_types_in_order=None, delimiter=',',
                  data_type='csv', has_header=True, line_index=None, skip_empty_line=False, sheet_name=0,
                  skip_rows=None
                  ):
         
         if data_link is not None:
             if data_type == 'csv':
                 if has_header is True:
-                    self.__dataframe = pd.read_csv(data_link, encoding='utf-8', delimiter=delimiter, 
+                    self.dataframe = pd.read_csv(data_link, encoding='utf-8', delimiter=delimiter, 
                                                low_memory=False, error_bad_lines=False, skip_blank_lines=False,
                                                skiprows=skip_rows)
                 else:
-                    self.__dataframe = pd.read_csv(data_link, encoding='utf-8', delimiter=delimiter, 
+                    self.dataframe = pd.read_csv(data_link, encoding='utf-8', delimiter=delimiter, 
                                                low_memory=False, error_bad_lines=False, skip_blank_lines=False,
                                                header=None)
             elif data_type == 'json':
-                self.__dataframe = pd.read_json(data_link, encoding='utf-8')
+                self.dataframe = pd.read_json(data_link, encoding='utf-8')
             elif data_type == 'xls':
-                self.__dataframe = pd.read_excel(data_link, sheet_name=sheet_name,
+                self.dataframe = pd.read_excel(data_link, sheet_name=sheet_name,
                                                  skiprows=skip_rows)
             elif data_type == 'pkl':
-                self.__dataframe = pd.read_pickle(data_link)
+                self.dataframe = pd.read_pickle(data_link)
             elif data_type == 'dict':
-                self.__dataframe = pd.DataFrame.from_dict(data_link)
+                self.dataframe = pd.DataFrame.from_dict(data_link)
             elif data_type == 'matrix':
                 index_name = [i for i in range(len(data_link))]
                 colums_name = [i for i in range(len(data_link[0]))]
-                self.__dataframe = pd.DataFrame(data=data_link, index=index_name, columns=colums_name)
+                self.dataframe = pd.DataFrame(data=data_link, index=index_name, columns=colums_name)
             elif data_type == 'list':
                 y = data_link
                 if (not isinstance(y, pd.core.series.Series or not isinstance(y, pd.core.frame.DataFrame))):
                     y = np.array(y)
                     y = np.reshape(y, (y.shape[0],))
                     y = pd.Series(y)
-                self.__dataframe = pd.DataFrame()
+                self.dataframe = pd.DataFrame()
                 if columns_names_as_list is not None:
-                    self.__dataframe[columns_names_as_list[0]] = y
+                    self.dataframe[columns_names_as_list[0]] = y
                 else:
-                    self.__dataframe['0'] = y
+                    self.dataframe['0'] = y
                     
                 
                 """data = array([['','Col1','Col2'],['Row1',1,2],['Row2',3,4]])
                 pd.DataFrame(data=data[1:,1:], index=data[1:,0], columns=data[0,1:]) """
             elif data_type == 'df':
-                self.__dataframe = data_link
+                self.dataframe = data_link
             types = {}
             if data_types_in_order is not None and columns_names_as_list is not None:
-                self.__dataframe.columns = columns_names_as_list
+                self.dataframe.columns = columns_names_as_list
                 for i in range(len(columns_names_as_list)):
                     types[columns_names_as_list[i]] = data_types_in_order[i]
             elif columns_names_as_list is not None:
-                self.__dataframe.columns = columns_names_as_list
+                self.dataframe.columns = columns_names_as_list
                 for p in columns_names_as_list:
                     types[p] = str
 
-            self.__dataframe = self.get_dataframe().astype(types)
+            self.dataframe = self.get_dataframe().astype(types)
 
             if line_index is not None:
-                self.__dataframe.index = line_index
+                self.dataframe.index = line_index
         else:
-            self.__dataframe = pd.DataFrame()
+            self.dataframe = pd.DataFrame()
         
     def get_generator(self):
         return self.__generator
     
     def remove_stopwords(self, column, language_or_stopwords_list='english', in_place=True):
         if isinstance(language_or_stopwords_list, list) is True:
             stopwords = language_or_stopwords_list
         elif language_or_stopwords_list == 'arabic':
             stopwords = Lib.read_text_file_as_list('data/arabic_stopwords.csv')
         else:
             nltk.download('stopwords')
             stopwords = nltk.corpus.stopwords.words(language_or_stopwords_list)
         self.transform_column(column, column, DataFrame.remove_stopwords_lambda, in_place, stopwords)
-        return self.__dataframe
+        return self.dataframe
     
     @staticmethod
     def remove_stopwords_lambda(document, stopwords_list):
         document = str.lower(document)
         stopwords = stopwords_list
         words = word_tokenize(document)
         clean_words = []
@@ -120,60 +121,60 @@
         elif distrubution_type == 'standard_normal':
             series = pd.Series(np.random.standard_normal(self.get_shape()[0]))
         elif distrubution_type == 'normal':
             series = pd.Series(np.random.normal(mean, sd, self.get_shape()[0]))
         else:
             series = pd.Series(np.random.randn(self.get_shape()[0]))
         self.add_column(column_name, series)
-        return self.__dataframe
+        return self.dataframe
     
     def drop_full_nan_columns(self):
-        for c in self.__dataframe.columns:
-                miss = self.__dataframe[c].isnull().sum()
+        for c in self.dataframe.columns:
+                miss = self.dataframe[c].isnull().sum()
                 missing_data_percent = round((miss/self.get_shape()[0])*100, 2)
                 if missing_data_percent == 100:
                     self.drop_column(c)
                     
     def drop_columns_with_nan_threshold(self, threshold=0.5):
-        for c in self.__dataframe.columns:
-                miss = self.__dataframe[c].isnull().sum()
+        for c in self.dataframe.columns:
+                miss = self.dataframe[c].isnull().sum()
                 missing_data_percent = round((miss/self.get_shape()[0])*100, 2)
                 if missing_data_percent >= threshold*100:
                     self.drop_column(c)
     
     def get_index(self, as_list=True):
         if as_list is True:
-            return self.__dataframe.index.to_list()
-        return self.__dataframe.index
+            return self.dataframe.index.to_list()
+        return self.dataframe.index
     
     def add_time_serie_row(self, date_column, value_column, value, date_format='%Y'):
         last_date = self.get_index()[-1] + timedelta(days=1)
         dataframe = DataFrame([{value_column: value, date_column: last_date}], data_type='dict')
         dataframe.to_time_series(date_column, value_column, one_row=True, date_format=date_format)
         self.append_dataframe(dataframe.get_dataframe())
         
     def set_generator(self, generator):
         self.__generator = generator
 
     def set_dataframe(self, data, data_type='df'):
         if data_type == 'matrix':
             index_name = [i for i in range(len(data))]
             colums_name = [i for i in range(len(data[0]))]
-            self.__dataframe = pd.DataFrame(data=data, index=index_name, columns=colums_name)
+            self.dataframe = pd.DataFrame(data=data, index=index_name, columns=colums_name)
         elif data_type == 'df':
-            self.__dataframe = data
+            self.dataframe = data
 
     def get_columns_types(self, show=True):
         types = self.get_dataframe().dtypes
         if show:
             print(types)
         return types
     
     def set_data_types(self, column_dict_types):
-        self.__dataframe = self.get_dataframe().astype(column_dict_types)
+        self.dataframe = self.get_dataframe().astype(column_dict_types)
         
     def set_same_type(self, same_type='float64'):
         """
         example of types: float64, object
         """
         for p in self.get_columns_names():
             self.set_column_type(p, same_type)
@@ -182,29 +183,29 @@
         description = self.get_dataframe().describe()
         if show:
             print(description)
         return description
     
     def reset_index(self, drop=True):
         if drop is True:
-            self.set_dataframe(self.__dataframe.reset_index(drop=True))
+            self.set_dataframe(self.dataframe.reset_index(drop=True))
         else:
-            self.set_dataframe(self.__dataframe.reset_index())
+            self.set_dataframe(self.dataframe.reset_index())
             
     def get_dataframe_as_sparse_matrix(self):
-        return scipy.sparse.csr_matrix(self.__dataframe.to_numpy())
+        return scipy.sparse.csr_matrix(self.dataframe.to_numpy())
 
     def get_column_as_list(self, column):
         return list(self.get_column(column))
     
     def get_column_as_joined_text(self, column):
         return ' '.join(list(self.get_column(column)))
     
     def rename_index(self, new_name):
-        self.__dataframe.index.rename(new_name, inplace=True)
+        self.dataframe.index.rename(new_name, inplace=True)
         return self.get_dataframe()
 
     def get_term_doc_matrix_as_df(self, text_column_name, vectorizer_type='count'):
         corpus = list(self.get_column(text_column_name))
         indice = ['doc' + str(i) for i in range(len(corpus))]
         v = Vectorizer(corpus, vectorizer_type=vectorizer_type)
         self.set_dataframe(DataFrame(v.get_sparse_matrix().toarray(), v.get_features_names(),
@@ -233,24 +234,24 @@
         data = DataFrame(counter.most_common(most_common), ['term', 'count'], data_type='dict', data_types_in_order=[str,int])
         chart = Chart(data.get_dataframe(), column4x='term', chart_type='bar')
         chart.add_data_to_show('count')
         chart.config('Term occurrences bar chart', 'Terms', 'Occurrences', titile_font_size=30,)
         chart.show()
 
     def set_dataframe_index(self, liste_indices):
-        self.__dataframe.index = liste_indices
+        self.dataframe.index = liste_indices
 
     def get_shape(self):
-        return self.__dataframe.shape
+        return self.dataframe.shape
 
     def set_column(self, column_name, new_column):
-        self.__dataframe[column_name] = new_column
+        self.dataframe[column_name] = new_column
 
     def set_column_type(self, column, column_type):
-        self.__dataframe[column] = self.__dataframe[column].astype(column_type)
+        self.dataframe[column] = self.dataframe[column].astype(column_type)
 
     def get_lines_columns(self, lines, columns):
         if Lib.check_all_elements_type(columns, str):
             return self.get_dataframe().loc[lines, columns]
         return self.get_dataframe().iloc[lines, columns]
     
     def get_n_rows_as_dataframe(self, number_of_row=10):
@@ -263,67 +264,94 @@
             return self.get_dataframe().head(number_of_row)
 
     def get_column(self, column):
         return self.get_dataframe()[column]
     
     def get_columns(self, columns_names_as_list):
         return self.get_dataframe()[columns_names_as_list]
+    
+    def add_noise(self, column_name, num_noises=100):
+        """
+        Adds random noise to a Pandas time series.
+        
+        Parameters:
+        ts (pandas.Series): the time series to which to add noise
+        num_noises (int): the number of noise values to add to the time series
+        
+        Returns:
+        pandas.Series: the time series with noise added
+        """
+        # Calculate the range of the time series data
+        data_range = self.get_column(column_name).max() - self.get_column(column_name).min()
+        
+        # Add the specified number of random noise values
+        for i in range(num_noises):
+            # Generate a random index within the time series
+            rand_index = self.dataframe.sample().index[0]
+            
+            # Generate a random noise value within the data range
+            noise_value = np.random.uniform(low=-data_range, high=data_range)
+            
+            # Add the noise value to the time series at the random date
+            self.set_row(column_name, rand_index, noise_value)
+        
+        return 0
 
     def rename_columns(self, column_dict_or_all_list, all_columns=False):
         if all_columns is True:
             types = {}
-            self.__dataframe.columns = column_dict_or_all_list
+            self.dataframe.columns = column_dict_or_all_list
             for p in column_dict_or_all_list:
                 types[p] = str
-            self.__dataframe = self.get_dataframe().astype(types)
+            self.dataframe = self.get_dataframe().astype(types)
         else:
             self.get_dataframe().rename(columns=column_dict_or_all_list, inplace=True) 
 
     def add_column(self, column_name, column):
         y = column
         if (not isinstance(column, pd.core.series.Series or not isinstance(column, pd.core.frame.DataFrame))):
             y = np.array(column)
             y = np.reshape(y, (y.shape[0],))
             if len(self.get_index()) == 0:
                 y = pd.Series(y)
             else:
                 y = pd.Series(y, self.get_index())
-        self.__dataframe[column_name] = y
+        self.dataframe[column_name] = y
         
     def add_transformed_columns(self, dest_column_name="new_column", transformation_rule="okk*2"):
         columns_names = self.get_columns_names()
         columns_dict = {}
         operations = {'sqrt': sqrt, 
          'pow': power,
          'exp': exp,
          }
         columns_dict.update(operations)
         for column_name in columns_names:
             if column_name in transformation_rule:
                 columns_dict.update({column_name: self.get_column(column_name)})
         y_transformed = eval(transformation_rule, columns_dict)
-        self.__dataframe[dest_column_name] = y_transformed
+        self.dataframe[dest_column_name] = y_transformed
         
     def add_one_value_column(self, column_name, value, length=None):
         if length is not None:
             y = np.zeros(length)
             y.fill(value)
         else:
             y = np.zeros((self.get_shape()[0]))
             y.fill(value)
-        self.__dataframe[column_name] = y
+        self.dataframe[column_name] = y
         return self.get_dataframe()
         
     def get_dataframe(self):
-        return self.__dataframe
+        return self.dataframe
 
     def request(self, select, order_by=None, ascending=None):
         if order_by is not None:
-            self.__dataframe = self.__dataframe.sort_values(order_by, ascending=ascending)
-        return self.__dataframe[select]
+            self.dataframe = self.dataframe.sort_values(order_by, ascending=ascending)
+        return self.dataframe[select]
 
     def contains(self, column, regex):
         return self.get_dataframe()[column].str.contains(regex)
 
     def to_upper_column(self, column):
         self.set_column(column, self.get_column(column).str.upper())
         
@@ -335,90 +363,90 @@
         self.add_column(new_date_time_column_name, self.get_column(date_column_name).astype(str) + ' ' + self.get_column(time_column_name).astype(str))
         self.column_to_date(new_date_time_column_name, format=date_time_format)
         
     def to_lower_column(self, column):
         self.set_column(column, self.get_column(column).str.lower())
 
     def sub(self, column, pattern, replacement):
-        self.__dataframe = self.get_dataframe()[column].str.replace(pattern, replacement)
+        self.dataframe = self.get_dataframe()[column].str.replace(pattern, replacement)
 
     def drop_column(self, column_name):
         """Drop a given column from the dataframe given its name
 
         Args:
             column (str): name of the column to drop
 
         Returns:
             [dataframe]: the dataframe with the column dropped
         """
-        self.__dataframe = self.__dataframe.drop(column_name, axis=1)
-        return self.__dataframe
+        self.dataframe = self.dataframe.drop(column_name, axis=1)
+        return self.dataframe
         
     def index_to_column(self, column_name=None):
-        self.__dataframe.reset_index(drop=False, inplace=True) 
+        self.dataframe.reset_index(drop=False, inplace=True) 
         if column_name is not None:
             self.rename_columns({'index': column_name})
         
     def drop_columns(self, columns_names_as_list):
         for p in columns_names_as_list:
-            self.__dataframe = self.__dataframe.drop(p, axis=1)
-        return self.__dataframe
+            self.dataframe = self.dataframe.drop(p, axis=1)
+        return self.dataframe
     
     def reorder_columns(self, new_order_as_list):
-        self.__dataframe.reindex_axis(new_order_as_list, axis=1)
-        return self.__dataframe
+        self.dataframe.reindex_axis(new_order_as_list, axis=1)
+        return self.dataframe
             
     def keep_columns(self, columns_names_as_list):
         for p in self.get_columns_names():
             if p not in columns_names_as_list:
-                self.__dataframe = self.__dataframe.drop(p, axis=1)
-        return self.__dataframe
+                self.dataframe = self.dataframe.drop(p, axis=1)
+        return self.dataframe
 
     def add_row(self, row_as_dict, index=None):
         if index is not None:
             row = pd.DataFrame(row_as_dict, index=[index])
-            self.__dataframe = pd.concat([self.__dataframe.iloc[:index], row, self.__dataframe.iloc[index:]]).reset_index(drop=True)
+            self.dataframe = pd.concat([self.dataframe.iloc[:index], row, self.dataframe.iloc[index:]]).reset_index(drop=True)
             #self.reset_index()
         else:
-            self.__dataframe = self.get_dataframe().append(row_as_dict, ignore_index=True)
+            self.dataframe = self.get_dataframe().append(row_as_dict, ignore_index=True)
 
     def pivot(self, index_columns_as_list, column_columns_as_list, column_of_values, agg_func):
         return self.get_dataframe().pivot_table(index=index_columns_as_list, columns=column_columns_as_list, values=column_of_values, aggfunc=agg_func)
 
     def group_by(self, column_name):
         self.set_dataframe(self.get_dataframe().groupby(column_name).count())
         
     def get_nan_indexes_of_column(self, column_name):
         return list(self.get_dataframe().loc[pd.isna(self.get_column(column_name)), :].index)
         
     def missing_data_checking(self, column_name=None):
         if column_name is not None:
             if any(pd.isna(self.get_dataframe()[column_name])) is True:
-                miss = self.__dataframe[column_name].isnull().sum()
+                miss = self.dataframe[column_name].isnull().sum()
                 missing_data_percent = round((miss/self.get_shape()[0])*100, 2)
                 print("{} has {} missing value(s) which represents {}% of dataset size".format(column_name, miss, missing_data_percent))
             else:
                 print("No missed data in column " + column_name)
         else:
             miss = []
-            for c in self.__dataframe.columns:
-                miss_by_column = self.__dataframe[c].isnull().sum()
+            for c in self.dataframe.columns:
+                miss_by_column = self.dataframe[c].isnull().sum()
                 if miss_by_column>0:
                     missing_data_percent = round((miss_by_column/self.get_shape()[0])*100, 2)
                     print("{} has {} missing value(s) which represents {}% of dataset size".format(c, miss_by_column, missing_data_percent))
                 else:
                     print("{} has NO missing value!".format(c))
                 miss.append(miss_by_column)
         return miss
     
     def missing_data_column_percent(self, column_name):
-        return self.__dataframe[column_name].isnull().sum()/self.get_shape()[0]
+        return self.dataframe[column_name].isnull().sum()/self.get_shape()[0]
     
     def get_missing_data_indexes_in_column(self, column_name):
-        return self.__dataframe[self.__dataframe[column_name].isnull()].index.tolist()
+        return self.dataframe[self.dataframe[column_name].isnull()].index.tolist()
 
     def missing_data(self, drop_row_if_nan_in_column=None, filling_dict_colmn_val=None, method='ffill',
                      column_to_fill='Ta', date_column_name=None):
         if filling_dict_colmn_val is None and drop_row_if_nan_in_column is None:
             if method == 'ffill':
                 self.get_dataframe().fillna(method='pad', inplace=True)
             elif method == 'bfill':
@@ -569,42 +597,42 @@
         
         if filling_dict_colmn_val is not None:
             self.get_dataframe().fillna(filling_dict_colmn_val, inplace=True)
             
         if drop_row_if_nan_in_column is not None:
             if drop_row_if_nan_in_column == 'all':
                 for p in self.get_columns_names():
-                    self.set_dataframe(self.__dataframe[self.__dataframe[p].notna()])
+                    self.set_dataframe(self.dataframe[self.dataframe[p].notna()])
             else:
                 # a = a[~(np.isnan(a).all(axis=1))] # removes rows containing all nan
-                self.set_dataframe(self.__dataframe[self.__dataframe[drop_row_if_nan_in_column].notna()])
-                #self.__dataframe = self.__dataframe[~(np.isnan(self.__dataframe).any(axis=1))] # removes rows containing at least one nan
+                self.set_dataframe(self.dataframe[self.dataframe[drop_row_if_nan_in_column].notna()])
+                #self.dataframe = self.dataframe[~(np.isnan(self.dataframe).any(axis=1))] # removes rows containing at least one nan
           
        
             
         
     def get_row(self, row_index):
         if isinstance(row_index, int):
             return self.get_dataframe().iloc[row_index]
         return self.get_dataframe().loc[row_index]
     
     def set_row(self, column_name, row_index, new_value):
         if isinstance(row_index, int):
-            self.__dataframe[column_name].iloc[row_index] = new_value
-        self.__dataframe[column_name].loc[row_index] = new_value
+            self.dataframe[column_name].iloc[row_index] = new_value
+        self.dataframe[column_name].loc[row_index] = new_value
     
     def replace_column(self, column, pattern, replacement, regex=False, number_of_time=-1, case_sensetivity=False):
         self.set_column(column, self.get_column(column).str.replace(pattern, replacement, regex=regex, n=number_of_time,
                                                                     case=case_sensetivity))
 
     def replace_num_data(self, val, replacement):
         self.get_dataframe().replace(val, replacement, inplace=True)
 
     def map_function(self, func, **kwargs):
-        self.__dataframe = self.get_dataframe().applymap(func, **kwargs)
+        self.dataframe = self.get_dataframe().applymap(func, **kwargs)
 
     def apply_fun_to_column(self, column, func, in_place=True,):
         if in_place is True:
             self.set_column(column, self.get_column(column).apply(func))
         else:
             return self.get_column(column).apply(func)
         
@@ -628,36 +656,36 @@
         """conacatenate horizontally two dataframe
 
         Args:
             dataframe (dataframe): the destination dataframe 
             ignore_index (bool, optional): If True, do not use the index values along the concatenation axis. Defaults to False.
         """
         # 
-        self.__dataframe = pd.concat([self.get_dataframe(), dataframe], axis=1, ignore_index=ignore_index, join=join)
+        self.dataframe = pd.concat([self.get_dataframe(), dataframe], axis=1, ignore_index=ignore_index, join=join)
     
     def append_dataframe(self, dataframe):
         # append dataset contents data_sets must have the same columns names
-        self.__dataframe = self.__dataframe.append(dataframe)
+        self.dataframe = self.dataframe.append(dataframe)
 
-    def join(self, dataframe, on_column='index'):
+    def join(self, dataframe, on_column='index', how='inner'):
         if on_column == 'index':
-           self.__dataframe = pd.merge(self.get_dataframe(), dataframe, left_index=True, right_index=True)
+           self.dataframe = pd.merge(self.get_dataframe(), dataframe, left_index=True, right_index=True, how=how)
         else:
-            self.__dataframe = pd.merge(self.__dataframe, dataframe, on=on_column, how='inner')
+            self.dataframe = pd.merge(self.dataframe, dataframe, on=on_column, how=how)
 
     def left_join(self, dataframe, column):
-        self.__dataframe = pd.merge(self.__dataframe, dataframe, on=column, how='left')
+        self.dataframe = pd.merge(self.dataframe, dataframe, on=column, how='left')
 
     def right_join(self, dataframe, column):
-        self.__dataframe = pd.merge(self.__dataframe, dataframe, on=column, how='right')
+        self.dataframe = pd.merge(self.dataframe, dataframe, on=column, how='right')
 
     def eliminate_outliers_neighbors(self, n_neighbors=20, contamination=.05):
         outliers = LocalOutlierFactor(n_neighbors=n_neighbors, contamination=contamination)
-        self.__dataframe['inlier'] = outliers.fit_predict(self.get_dataframe())
-        self.__dataframe = self.get_dataframe().loc[self.get_dataframe().inlier == 1,
+        self.dataframe['inlier'] = outliers.fit_predict(self.get_dataframe())
+        self.dataframe = self.get_dataframe().loc[self.get_dataframe().inlier == 1,
                                                       self.get_dataframe().columns.tolist()]
 
     def get_pca(self, new_dim):
         # pca.explained_variance_ratio_ gain d'info pour chaque vecteur
         pca_model = PCA(n_components=new_dim)
         return pca_model.fit_transform(self.get_dataframe())
 
@@ -819,23 +847,73 @@
         else:
             self.apply_fun_to_column(column, lambda x: list(map(str.lower, x.split(' '))).count(value))
             return self.get_column(column).sum()
 
     def count_true_decision_function_rows(self, column, decision_function):
         self.filter_dataframe(column, decision_function)
         
+    def add_artificial_missing_data(self, column_name, nbr_missing_data=31, method='continious'):
+        """
+        Fill a randomly selected period with NaN values in a specified column of a pandas dataframe.
+
+        Parameters:
+            df (pandas.DataFrame): The input dataframe.
+            column (str): The name of the column to fill with NaN values.
+            period (str): The length of the period to fill with NaN values, in pandas frequency string format (e.g., 'D' for day, 'W' for week, 'M' for month).
+
+        Returns:
+            None
+        """
+        
+        filled_indices = []
+        if method == 'continious':
+            random_index = self.dataframe.sample().index[0]
+            #self.dataframe[random_index:random_index+nbr_missing_data][column_name] = np.nan 
+            previous_data = self.dataframe.loc[(self.dataframe.index >= random_index) & (self.dataframe.index < random_index + nbr_missing_data), column_name]
+            self.dataframe.loc[(self.dataframe.index >= random_index) & (self.dataframe.index < random_index + nbr_missing_data), column_name] = np.nan
+            # Fill the selected period with NaN values in the specified column
+            #df.loc[(df.index >= random_period) & (df.index < random_period + pd.Timedelta(period)), column] = np.nan
+            filled_indices = range(random_index, random_index + nbr_missing_data) 
+        else:
+            for  i in range(nbr_missing_data):
+                random_index = self.dataframe.sample().index[0]
+                self.dataframe.loc[self.dataframe.index == random_index, column_name] = np.nan
+                filled_indices.append(random_index)
+        return previous_data
+            
     def plot_column(self, column_name, x_column_name='index', 
                     x_label='Date & time',
                     y_label=None,
                     x_label_rotation=0,
                     y_label_rotation=0,
                     save_fig=False,
-                    savefig_path='out.png'
+                    savefig_path='out.png',
+                    date_format_x_axis=None
                     ):
+        """_summary_
+
+        Args:
+            column_name (_type_): _description_
+            x_column_name (str, optional): _description_. Defaults to 'index'.
+            x_label (str, optional): _description_. Defaults to 'Date & time'.
+            y_label (_type_, optional): _description_. Defaults to None.
+            x_label_rotation (int, optional): _description_. Defaults to 0.
+            y_label_rotation (int, optional): _description_. Defaults to 0.
+            save_fig (bool, optional): _description_. Defaults to False.
+            savefig_path (str, optional): _description_. Defaults to 'out.png'.
+            date_format_x_axis (str, optional): _description_. Example to '%m-%d'.
+        """
         fig, ax = plt.subplots()
+        
+        if date_format_x_axis is not None:
+            import matplotlib.dates as mdate
+            # format the x-axis tick labels
+            date_format = mdate.DateFormatter(date_format_x_axis)
+            ax.xaxis.set_major_formatter(date_format)
+            
         if x_column_name == 'index':
             ax.plot(self.get_index(), self.get_column(column_name))
         else:
             ax.plot(self.get_column(x_column_name), self.get_column(column_name))
         # set the axis labels and title
         ax.set_xlabel(x_label)
         if y_label is None:
@@ -847,16 +925,16 @@
         if save_fig is True:
             import matplotlib as mpl
             mpl.rcParams['agg.path.chunksize'] = 10000
             fig.savefig(savefig_path, dpi=720)
         plt.show()
         
     def split_export(self, percentage=0.8, train_out_file="train.csv", test_out_file="test.csv"):
-        train = self.__dataframe.iloc[:int(percentage*self.get_shape()[0]), :]
-        test = self.__dataframe.iloc[int(percentage*self.get_shape()[0]):, :]
+        train = self.dataframe.iloc[:int(percentage*self.get_shape()[0]), :]
+        test = self.dataframe.iloc[int(percentage*self.get_shape()[0]):, :]
         train.to_csv(train_out_file, index=False)
         test.to_csv(test_out_file, index=False) 
         
     def show_wordcloud(self, column):
         wordcloud = WordCloud(
             background_color='white',
             max_words=100,
@@ -871,15 +949,15 @@
         plt.show()
 
     def reindex_dataframe(self, index_as_column_name=None, index_as_liste=None):
         if index_as_liste is not None:
             new_index = new_index = index_as_liste
             self.get_dataframe().index = new_index
         if index_as_column_name is not None:
-            self.__dataframe.set_index(index_as_column_name, inplace=True)
+            self.dataframe.set_index(index_as_column_name, inplace=True)
         if index_as_column_name is None and index_as_liste is None:
             new_index = pd.Series(np.arange(self.get_shape()[0]))
             self.get_dataframe().index = new_index
     
     def get_columns_names(self):
         header = list(self.get_dataframe().columns)
         return header 
@@ -957,38 +1035,38 @@
         self.filter_dataframe(column, self.outliers_decision_function, min_q, max_q)
 
     def scale_column(self, column):
         max_column = self.get_column(column).describe()['max']
         self.transform_column(column, column, self.scale_trasform_fun, max_column)
 
     def drop_duplicated_rows(self, column):
-        self.set_dataframe(self.__dataframe.drop_duplicates(subset=column, keep='first'))
+        self.set_dataframe(self.dataframe.drop_duplicates(subset=column, keep='first'))
         
     def drop_duplicated_indexes(self):
-        self.__dataframe = self.__dataframe[~self.__dataframe.index.duplicated(keep='first')]
+        self.dataframe = self.dataframe[~self.dataframe.index.duplicated(keep='first')]
         
     def plot_dataframe(self):
         self.get_dataframe().plot()
         plt.show()
         
     def to_numpy(self):
         return self.get_dataframe().values
     
-    def generate_datetime_range_dataframe(self, 
-                                          starting_datetime='2013-01-01 00:00:00', 
+    @staticmethod
+    def generate_datetime_range_dataframe(starting_datetime='2013-01-01 00:00:00', 
                                           end_datetime='2013-12-31 00:00:00', 
                                           periods=None, 
                                           freq='1H'):
-        self.__dataframe = DataFrame().get_dataframe()
-        self.set_dataframe_index(self.generate_datetime_range(
-            starting_datetime='2013-01-01 00:00:00', 
-            end_datetime='2013-12-31 00:00:00', 
-            periods=None, 
-            freq='1H'))
-        return self.get_dataframe()
+        dataframe = DataFrame()
+        dataframe.set_dataframe_index(DataFrame.generate_datetime_range(
+            starting_datetime=starting_datetime, 
+            end_datetime=end_datetime, 
+            periods=periods,
+            freq=freq))
+        return dataframe.get_dataframe()
     
     def info(self):
         return self.get_dataframe().info()
     
     def drop_rows_by_year(self, year=2020, in_place=True):
         year = int(year)
         if in_place is True:
@@ -1164,70 +1242,77 @@
         
         if method == 'pm':
             et0_data.add_column_based_on_function('et0_pm', DataFrame.et0_penman_monteith)
         elif method == 'hargreaves':
             et0_data.add_column_based_on_function('et0_hargreaves', DataFrame.et0_hargreaves)
             
         if in_place == True:
-            self.__dataframe = et0_data.get_dataframe()
+            self.dataframe = et0_data.get_dataframe()
             
         return et0_data.get_dataframe()
         
         
     def column_to_date(self, column, format='%Y-%m-%d %H:%M:%S'):
         self.set_column(column, pd.to_datetime(self.get_column(column)))
         self.set_column(column, self.get_column(column).dt.strftime(format))
         self.set_column(column, pd.to_datetime(self.get_column(column)))
         
     def date_time_formate(self, date_time_column_name, new_format='%Y-%m-%d %H:%M:%S'):
         self.set_column(date_time_column_name, self.get_column(date_time_column_name).dt.strftime(new_format))
         return self.get_dataframe()
 
     def resample_timeseries(self, 
-                            date_column_name='date_time',
-                            frequency='d', agg='mean', 
+                            frequency='d', 
+                            agg='mean', 
                             skip_rows=None, 
                             intitial_index=0, 
-                            reset_index=False,
                             between_time_tuple=None,
+                            date_column_name=None,
                             in_place=True):
         if in_place is True:
             if skip_rows is not None:
                 self.set_dataframe(self.get_dataframe().loc[intitial_index:self.get_shape()[0]:skip_rows])
+                self.reset_index()
             else:
-                self.reindex_dataframe(date_column_name)
+                if date_column_name is not None:
+                    self.reindex_dataframe(date_column_name)
+                    
+                if between_time_tuple is not None:
+                    temp_time_series = temp_time_series.between_time(between_time_tuple[0], between_time_tuple[1])
+                    
                 if agg == 'sum':
-                    self.set_dataframe(self.__dataframe.resample(frequency).sum())
+                    self.set_dataframe(self.dataframe.resample(frequency).sum())
                 if agg == 'mean':
-                    self.set_dataframe(self.__dataframe.resample(frequency).mean())
+                    self.set_dataframe(self.dataframe.resample(frequency).mean())
                 if agg == 'max':
-                    self.set_dataframe(self.__dataframe.resample(frequency).max())
+                    self.set_dataframe(self.dataframe.resample(frequency).max())
                 if agg == 'min':
-                    self.set_dataframe(self.__dataframe.resample(frequency).min())
+                    self.set_dataframe(self.dataframe.resample(frequency).min())
                 if agg == 'median':
-                    self.set_dataframe(self.__dataframe.resample(frequency).median())
+                    self.set_dataframe(self.dataframe.resample(frequency).median())
                 if agg == 'std':
-                    self.set_dataframe(self.__dataframe.resample(frequency).std())
+                    self.set_dataframe(self.dataframe.resample(frequency).std())
                 if agg == 'var':
-                    self.set_dataframe(self.__dataframe.resample(frequency).var())
+                    self.set_dataframe(self.dataframe.resample(frequency).var())
                 if agg == 'ffill':
-                    self.set_dataframe(self.__dataframe.resample(frequency).ffill())
+                    self.set_dataframe(self.dataframe.resample(frequency).ffill())
                 if agg == 'bfill':
-                    self.set_dataframe(self.__dataframe.resample(frequency).bfill())
+                    self.set_dataframe(self.dataframe.resample(frequency).bfill())
                 else:
-                    self.set_dataframe(self.__dataframe.resample(frequency).mean())
-            if reset_index is True:
-                self.reset_index()
+                    self.set_dataframe(self.dataframe.resample(frequency).mean())
             return self.get_dataframe()
         else:
             if skip_rows is not None:
                 self.set_dataframe(self.get_dataframe().loc[intitial_index:self.get_shape()[0]:skip_rows])
             else:
-                self.reindex_dataframe(date_column_name)
-                temp_time_series = self.__dataframe
+                if date_column_name is not None:
+                    self.reindex_dataframe(date_column_name)
+                    
+                temp_time_series = self.dataframe
+                
                 if between_time_tuple is not None:
                     temp_time_series = temp_time_series.between_time(between_time_tuple[0], between_time_tuple[1])
 
                 if agg == 'sum':
                     resampled_dataframe = temp_time_series.resample(frequency).sum()
                 if agg == 'mean':
                     resampled_dataframe = temp_time_series.resample(frequency).mean()
@@ -1241,18 +1326,15 @@
                     resampled_dataframe = temp_time_series.resample(frequency).std()
                 if agg == 'var':
                     resampled_dataframe = temp_time_series.resample(frequency).var()
                 if agg == 'ffill':
                     resampled_dataframe = temp_time_series.resample(frequency).ffill()
                 if agg == 'bfill':
                     resampled_dataframe = temp_time_series.resample(frequency).bfill()
-                
-                self.index_to_column('date_time')
-            if reset_index is True:
-                self.reset_index()
+            
             return resampled_dataframe
         
     def to_time_series(self, date_column, value_column, date_format='%Y-%m-%d', window_size=2, one_row=False):
         from tensorflow.keras.preprocessing.sequence import TimeseriesGenerator as SG
         # when working with train test generators
         """def to_time_series_generators(self, date_column, time_series_column, date_format='%Y-%m-%d', window_size=2, train_percent=0.8):
         self.column_to_date(date_column, format=date_format)
@@ -1320,14 +1402,17 @@
         
     def shuffle_dataframe(self):
         self.set_dataframe(self.get_dataframe().sample(frac=1).reset_index(drop=True))
         
     def add_doy_column(self, date_time_column_name='date_time'):
         self.add_column('doy', self.get_column(date_time_column_name).dt.day_of_year)
         
+    def add_month_day_column(self, date_time_column_name='date_time'):
+        self.add_column('month-day', self.get_column(date_time_column_name).dt.month.astype(str) + '-' + self.get_column(date_time_column_name).dt.day.astype(str))
+    
     def scale_columns(self, columns_names_as_list, scaler_type='min_max', in_place=True):
         """A method  to standardize the independent features present in the concerned columns in a fixed range.
 
         Args:
             column_name ([type]): 
             scaler_type (str, optional): ['min_max', 'standard', 'adjusted_log']. Defaults to 'min_max'.
             in_place (bool, optional): if False the modification do not  affects the original columns. Defaults to True.
@@ -1425,15 +1510,15 @@
     @staticmethod
     def outliers_decision_function(o, min_quantile, max_quantile):
         if min_quantile < o < max_quantile:
             return True
         return False
     
     @staticmethod
-    def generate_datetime_range(starting_datetime='2013-01-01 00:00:00', end_datetime='2013-12-31 00:00:00', periods=None, freq='1H'):
+    def generate_datetime_range(starting_datetime='2013-01-01 00:00:00', end_datetime='2013-12-31 00:00:00', freq='1H', periods=None):
         if periods is not None:
             return pd.date_range(start=starting_datetime, periods=periods, freq=freq)
         return pd.date_range(start=starting_datetime, end=end_datetime, freq=freq)
 
     @staticmethod
     def scale_trasform_fun(o, max_column):
         return o / max_column
```

### Comparing `data-science-toolkit-0.0.999/src/data_science_toolkit/gis.py` & `data-science-toolkit-0.1.0/src/data_science_toolkit/gis.py`

 * *Files identical despite different names*

### Comparing `data-science-toolkit-0.0.999/src/data_science_toolkit/imagefactory.py` & `data-science-toolkit-0.1.0/src/data_science_toolkit/imagefactory.py`

 * *Files identical despite different names*

### Comparing `data-science-toolkit-0.0.999/src/data_science_toolkit/lib.py` & `data-science-toolkit-0.1.0/src/data_science_toolkit/lib.py`

 * *Files identical despite different names*

### Comparing `data-science-toolkit-0.0.999/src/data_science_toolkit/model.py` & `data-science-toolkit-0.1.0/src/data_science_toolkit/model.py`

 * *Files identical despite different names*

### Comparing `data-science-toolkit-0.0.999/src/data_science_toolkit/r3.py` & `data-science-toolkit-0.1.0/src/data_science_toolkit/r3.py`

 * *Files identical despite different names*

### Comparing `data-science-toolkit-0.0.999/src/data_science_toolkit/rl.py` & `data-science-toolkit-0.1.0/src/data_science_toolkit/rl.py`

 * *Files identical despite different names*

### Comparing `data-science-toolkit-0.0.999/src/data_science_toolkit/rl_dqn.py` & `data-science-toolkit-0.1.0/src/data_science_toolkit/rl_dqn.py`

 * *Files identical despite different names*

### Comparing `data-science-toolkit-0.0.999/src/data_science_toolkit/vectorizer.py` & `data-science-toolkit-0.1.0/src/data_science_toolkit/vectorizer.py`

 * *Files identical despite different names*

### Comparing `data-science-toolkit-0.0.999/src/data_science_toolkit.egg-info/PKG-INFO` & `data-science-toolkit-0.1.0/src/data_science_toolkit.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data-science-toolkit
-Version: 0.0.999
+Version: 0.1.0
 Summary: Data Science Toolkit (DST) is a Python library that helps implement data science related project with ease.
 Home-page: https://github.com/elhachimi-ch/dst
 Author: EL HACHIMI CHOUAIB
 Author-email: elhachimi.ch@gmail.com
 Project-URL: Bug Tracker, https://github.com/elhachimi-ch/dst/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `data-science-toolkit-0.0.999/src/data_science_toolkit.egg-info/SOURCES.txt` & `data-science-toolkit-0.1.0/src/data_science_toolkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

