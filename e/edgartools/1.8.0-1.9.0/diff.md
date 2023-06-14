# Comparing `tmp/edgartools-1.8.0.tar.gz` & `tmp/edgartools-1.9.0.tar.gz`

## Comparing `edgartools-1.8.0.tar` & `edgartools-1.9.0.tar`

### file list

```diff
@@ -1,18 +1,20 @@
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 edgartools-1.8.0/edgar/__about__.py
--rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 edgartools-1.8.0/edgar/__init__.py
--rw-r--r--   0        0        0    27308 2020-02-02 00:00:00.000000 edgartools-1.8.0/edgar/company.py
--rw-r--r--   0        0        0    14500 2020-02-02 00:00:00.000000 edgartools-1.8.0/edgar/core.py
--rw-r--r--   0        0        0     6455 2020-02-02 00:00:00.000000 edgartools-1.8.0/edgar/effect.py
--rw-r--r--   0        0        0    34049 2020-02-02 00:00:00.000000 edgartools-1.8.0/edgar/filing.py
--rw-r--r--   0        0        0     3013 2020-02-02 00:00:00.000000 edgartools-1.8.0/edgar/form.py
--rw-r--r--   0        0        0     1378 2020-02-02 00:00:00.000000 edgartools-1.8.0/edgar/gaap.py
--rw-r--r--   0        0        0    27909 2020-02-02 00:00:00.000000 edgartools-1.8.0/edgar/ownership.py
--rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 edgartools-1.8.0/edgar/shelf.py
--rw-r--r--   0        0        0     8215 2020-02-02 00:00:00.000000 edgartools-1.8.0/edgar/xbrl.py
--rw-r--r--   0        0        0     2857 2020-02-02 00:00:00.000000 edgartools-1.8.0/edgar/xml.py
--rw-r--r--   0        0        0  1609032 2020-02-02 00:00:00.000000 edgartools-1.8.0/edgar/data/GAAP_Taxonomy_2022.csv
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 edgartools-1.8.0/.gitignore
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 edgartools-1.8.0/LICENSE.txt
--rw-r--r--   0        0        0    16017 2020-02-02 00:00:00.000000 edgartools-1.8.0/README.md
--rw-r--r--   0        0        0     2402 2020-02-02 00:00:00.000000 edgartools-1.8.0/pyproject.toml
--rw-r--r--   0        0        0    16854 2020-02-02 00:00:00.000000 edgartools-1.8.0/PKG-INFO
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 edgartools-1.9.0/edgar/__about__.py
+-rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 edgartools-1.9.0/edgar/__init__.py
+-rw-r--r--   0        0        0    27308 2020-02-02 00:00:00.000000 edgartools-1.9.0/edgar/company.py
+-rw-r--r--   0        0        0    14500 2020-02-02 00:00:00.000000 edgartools-1.9.0/edgar/core.py
+-rw-r--r--   0        0        0     6455 2020-02-02 00:00:00.000000 edgartools-1.9.0/edgar/effect.py
+-rw-r--r--   0        0        0    34049 2020-02-02 00:00:00.000000 edgartools-1.9.0/edgar/filing.py
+-rw-r--r--   0        0        0     3013 2020-02-02 00:00:00.000000 edgartools-1.9.0/edgar/form.py
+-rw-r--r--   0        0        0     1378 2020-02-02 00:00:00.000000 edgartools-1.9.0/edgar/gaap.py
+-rw-r--r--   0        0        0    21600 2020-02-02 00:00:00.000000 edgartools-1.9.0/edgar/offering.py
+-rw-r--r--   0        0        0    27135 2020-02-02 00:00:00.000000 edgartools-1.9.0/edgar/ownership.py
+-rw-r--r--   0        0        0     6013 2020-02-02 00:00:00.000000 edgartools-1.9.0/edgar/party.py
+-rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 edgartools-1.9.0/edgar/shelf.py
+-rw-r--r--   0        0        0     8215 2020-02-02 00:00:00.000000 edgartools-1.9.0/edgar/xbrl.py
+-rw-r--r--   0        0        0     2857 2020-02-02 00:00:00.000000 edgartools-1.9.0/edgar/xml.py
+-rw-r--r--   0        0        0  1609032 2020-02-02 00:00:00.000000 edgartools-1.9.0/edgar/data/GAAP_Taxonomy_2022.csv
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 edgartools-1.9.0/.gitignore
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 edgartools-1.9.0/LICENSE.txt
+-rw-r--r--   0        0        0    17441 2020-02-02 00:00:00.000000 edgartools-1.9.0/README.md
+-rw-r--r--   0        0        0     2402 2020-02-02 00:00:00.000000 edgartools-1.9.0/pyproject.toml
+-rw-r--r--   0        0        0    18229 2020-02-02 00:00:00.000000 edgartools-1.9.0/PKG-INFO
```

### Comparing `edgartools-1.8.0/edgar/__init__.py` & `edgartools-1.9.0/edgar/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,7 +14,8 @@
                         set_identity)
 from edgar.filing import (Filing,
                           Filings,
                           get_filings,
                           FilingHomepage)
 from edgar.ownership import Ownership
 from edgar.effect import Effect
+from edgar.offering import Offering
```

### Comparing `edgartools-1.8.0/edgar/company.py` & `edgartools-1.9.0/edgar/company.py`

 * *Files identical despite different names*

### Comparing `edgartools-1.8.0/edgar/core.py` & `edgartools-1.9.0/edgar/core.py`

 * *Files identical despite different names*

### Comparing `edgartools-1.8.0/edgar/effect.py` & `edgartools-1.9.0/edgar/effect.py`

 * *Files identical despite different names*

### Comparing `edgartools-1.8.0/edgar/filing.py` & `edgartools-1.9.0/edgar/filing.py`

 * *Files identical despite different names*

### Comparing `edgartools-1.8.0/edgar/form.py` & `edgartools-1.9.0/edgar/form.py`

 * *Files identical despite different names*

### Comparing `edgartools-1.8.0/edgar/gaap.py` & `edgartools-1.9.0/edgar/gaap.py`

 * *Files identical despite different names*

### Comparing `edgartools-1.8.0/edgar/ownership.py` & `edgartools-1.9.0/edgar/ownership.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from dataclasses import dataclass
-from typing import List, Dict, Optional, Tuple
+from typing import List, Dict, Tuple
 
 import pandas as pd
 from bs4 import BeautifulSoup
 from bs4 import Tag
 from rich.console import Group, Text
 from rich.panel import Panel
 
 from edgar.core import get_bool
 from edgar.core import repr_rich, df_to_rich_table, IntString
+from edgar.party import Address
 from edgar.xml import (child_text, child_value)
 
 __all__ = [
     'Owner',
     'Issuer',
     'Address',
     'Footnotes',
@@ -71,36 +72,14 @@
         self.name: str = name
         self.ticker: str = ticker
 
     def __repr__(self):
         return f"Issuer(cik='{self.cik or ''}', name={self.name or ''}, ticker={self.ticker or ''})"
 
 
-class Address:
-
-    def __init__(self,
-                 street1: str,
-                 street2: Optional[str] = None,
-                 city: Optional[str] = None,
-                 state: Optional[str] = None,
-                 zipcode: Optional[str] = None,
-                 state_description: Optional[str] = None
-                 ):
-        self.street1: str = street1
-        self.street2: Optional[str] = street2
-        self.city: Optional[str] = city
-        self.state: Optional[str] = state
-        self.zipcode: Optional[str] = zipcode
-        self.state_description: Optional[str] = state_description
-
-    def __repr__(self):
-        return (f"Address(street1='{self.street1}', street2={self.street2}, city={self.city}, "
-                f"zipcode={self.zipcode}, state={self.state})")
-
-
 class ReportingRelationship:
     """
     The relationship of the reporter to the company
     """
 
     def __init__(self,
                  is_director: bool,
@@ -725,17 +704,17 @@
         ) for el in root.find_all("ownerSignature")]
 
         reporting_owner_address_tag = reporting_owner_tag.find("reportingOwnerAddress")
         reporting_owner_address = Address(
             street1=child_text(reporting_owner_address_tag, "rptOwnerStreet1"),
             street2=child_text(reporting_owner_address_tag, "rptOwnerStreet2"),
             city=child_text(reporting_owner_address_tag, "rptOwnerCity"),
-            state=child_text(reporting_owner_address_tag, "rptOwnerState"),
+            state_or_country=child_text(reporting_owner_address_tag, "rptOwnerState"),
             zipcode=child_text(reporting_owner_address_tag, "rptOwnerZipCode"),
-            state_description=child_text(reporting_owner_address_tag, "rptOwnerStateDescription")
+            state_or_country_description=child_text(reporting_owner_address_tag, "rptOwnerStateDescription")
         )
 
         reporting_owner_rel_tag = reporting_owner_tag.find("reportingOwnerRelationship")
         reporting_relationship = ReportingRelationship(
             is_director=get_bool(child_text(reporting_owner_rel_tag, "isDirector")),
             is_officer=get_bool(child_text(reporting_owner_rel_tag, "isOfficer")),
             is_ten_pct_owner=get_bool(child_text(reporting_owner_rel_tag, "isTenPercentOwner")),
```

### Comparing `edgartools-1.8.0/edgar/xbrl.py` & `edgartools-1.9.0/edgar/xbrl.py`

 * *Files identical despite different names*

### Comparing `edgartools-1.8.0/edgar/xml.py` & `edgartools-1.9.0/edgar/xml.py`

 * *Files identical despite different names*

### Comparing `edgartools-1.8.0/edgar/data/GAAP_Taxonomy_2022.csv` & `edgartools-1.9.0/edgar/data/GAAP_Taxonomy_2022.csv`

 * *Files identical despite different names*

### Comparing `edgartools-1.8.0/LICENSE.txt` & `edgartools-1.9.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `edgartools-1.8.0/README.md` & `edgartools-1.9.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 
 
-![edgar-tools-logo](https://raw.githubusercontent.com/dgunning/edgartools/main/edgar-tools.png)
+![edgar-tools-logo](https://raw.githubusercontent.com/dgunning/edgartools/main/images/edgar-tools.png)
 
 [![PyPI - Version](https://img.shields.io/pypi/v/edgartools.svg)](https://pypi.org/project/edgartools)
 ![GitHub last commit](https://img.shields.io/github/last-commit/dgunning/edgartools)
 ![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/dgunning/edgartools/python-hatch-workflow.yml)
 [![CodeFactor](https://www.codefactor.io/repository/github/dgunning/edgartools/badge)](https://www.codefactor.io/repository/github/dgunning/edgartools)
 [![Hatch project](https://img.shields.io/badge/%F0%9F%A5%9A-Hatch-4051b5.svg)](https://github.com/pypa/hatch)
 ![GitHub](https://img.shields.io/github/license/dgunning/edgartools)
@@ -24,27 +24,28 @@
     <li>
         <a href="#installation">Installation</a>
     </li>
     <li>
         <a href="#usage">Usage</a>
         <ul>
             <li><a href="#setting-your-edgar-user-identity">Setting your Edgar user identity</a></li>
+            <li><a href="#getting-filings">Getting Filings</a></li>
             <li><a href="#using-the-company-api">Using the Company API</a></li>
-            <li><a href="#using-the-filings-api">Using the Filings API</a></li>
       </ul>
     </li>
     <li><a href="#contributing">Contributing</a></li>
     <li><a href="#license">License</a></li>
     <li><a href="#contact">Contact</a></li>
   </ol>
 </details>
 
 # About the project
 
-**`edgartools`** is a library for working Edgar filings in analytic workflows.
+**`edgartools`** is a library for working with SEC Edgar filings. You can query, filter and select any filing since 1994 and view the filing's html, text, xml or structured data.
+
 
 ## Demo
 
 #### Get the Common Shares Issued amount from Snowflake's latest 10-Q filing
 
 ```python
 (Company("SNOW")
@@ -56,15 +57,15 @@
            where fact = 'CommonStockSharesIssued' 
            order by end_date desc limit 1
         """
     ).df()
 )
 ```
 
-![Common Shares Issued](https://raw.githubusercontent.com/dgunning/edgartools/main/common-shares-issued.png)
+![Common Shares Issued](https://raw.githubusercontent.com/dgunning/edgartools/main/images/common-shares-issued.png)
 
 This example shows what can be done with **edgartools**.
 
 Under the hood the code does the following
 
 1. Use the ticker **"SNOW"** to get the company's cik from the [Company Tickers JSON](https://www.sec.gov/file/company-tickers)
 2. From the **cik** get the company's filings from the submissions endpoint `https://data.sec.gov/submissions/CIK{cik:010}.json`
@@ -122,17 +123,224 @@
 ```
 Alternatively, you can call `set_identity` which does the same thing.
 
 ```python
 from edgar import set_identity
 set_identity("Michael Mccallum mcalum@gmail.com")
 ```
+For more detail see https://www.sec.gov/os/accessing-edgar-data
 
 
-For more detail see https://www.sec.gov/os/accessing-edgar-data
+## Getting filings
+To get started import from edgar and use the `get_filings` function.
+```python
+from edgar import *
+
+filings = get_filings()
+```
+
+This gets the list of filings for the current year and quarter into a `Filings` object. 
+
+![Get Filings](https://raw.githubusercontent.com/dgunning/edgartools/main/images/get_filings.jpg)
+
+If you need a different date range you can specify a year or years and a quarter or quarters.
+These are valid ways to specify the date range or filter by form or by filing date.
+
+```python
+
+    >>> filings = get_filings(2021) # Get filings for 2021
+
+    >>> filings = get_filings(2021, 4) # Get filings for 2021 Q4
+
+    >>> filings = get_filings(2021, [3,4]) # Get filings for 2021 Q3 and Q4
+
+    >>> filings = get_filings([2020, 2021]) # Get filings for 2020 and 2021
+
+    >>> filings = get_filings([2020, 2021], 4) # Get filings for Q4 of 2020 and 2021
+
+    >>> filings = get_filings(range(2010, 2021)) # Get filings between 2010 and 2021 - does not include 2021
+
+    >>> filings = get_filings(2021, 4, form="D") # Get filings for 2021 Q4 for form D
+
+    >>> filings = get_filings(2021, 4, filing_date="2021-10-01") # Get filings for 2021 Q4 on "2021-10-01"
+
+    >>> filings = get_filings(2021, 4, filing_date="2021-10-01:2021-10-10") # Get filings for 2021 Q4 between
+                                                                            # "2021-10-01" and "2021-10-10"
+```
+
+### Convert the filings to a pandas dataframe
+
+The filings data is stored in the `Filings` class as a `pyarrow.Table`. You can get the data as a pandas dataframe using
+`to_pandas`
+```python
+df = filings.to_pandas()
+```
+
+
+## Navigating filings
+
+The Filings object allows you to navigate through filings using `filings.next()` and `filings.prev()`. 
+This shows you pages of the data - the page size is about 50. 
+
+```python
+# To see the next page of data
+filings.next()
+
+# To see the previous page
+filings.prev()
+
+# To see the current page
+filings.current()
+```
+
+![Get next filings](https://raw.githubusercontent.com/dgunning/edgartools/main/images/filings_next.jpg)
+
+## Getting the latest filings
+
+You can get the latest **n** filings by filing_date from a filings using `filings.latest()`.
+
+If you provide the parameter `n` it will return the latest `n` filings.
+
+```python
+filing = filings.latest(n=5)
+filing
+```
+![Latest filings](https://raw.githubusercontent.com/dgunning/edgartools/main/images/latest_filings.jpg)
+
+
+If you omit this parameter, or set `n=1` it will return a single `Filings object.
+
+```python
+filing = filings.latest()
+filing
+```
+![Latest filing](https://raw.githubusercontent.com/dgunning/edgartools/main/images/latest_filing.jpg)
+
+
+## Filtering filings
+
+You can filter the filings object using te `filter()` function. This allows you to filter
+by filing date, or by form.
+
+### Filtering filings by date
+
+To filter by filing date specify the filing date in **YYYY-MM-DD** format e.g. **2022-01-24**
+(Note the parameters `date` and `filing_date` are equivalent aliases for each other)
+```python
+filings.filter(date="2021-01-24") # or filings.filter(filing_date="2021-01-24")
+```
+You can specify a filing date range using the colon
+
+```python
+filings.filter(date="2021-01-12:2021-02-28") 
+```
+To filter by dates before a specified date use `:YYYY-MM-DD'
+
+```python
+filings.filter(date=":2021-02-28") 
+```
+
+To filter by dates after a specified date use `YYYY-MM-DD:'
+
+```python
+filings.filter(date="2021-02-28:") 
+```
+
+### Filtering filings by form
+
+You can filter filings by form using the `form` parameter. 
+
+```python
+filings.filter(form="10-K") 
+```
+
+To filter by form e.g. **10-K** and include form amendments use `amendments = True`. 
+
+```python
+filings.filter(form="10-K", amendments=True) 
+```
+![Filter with amendments](https://raw.githubusercontent.com/dgunning/edgartools/main/images/filter_amendments.jpg)
+
+## Getting a single filing
+
+You can get a single filing from the filings using the bracket operator `[]`, 
+specifying the index of the filing. The index is the value displayed in the leftmost
+position in the filings table. For example, to get the **10-Q** for **Costco** in the table above
+use `filings[3]`
+
+```python
+filing = filings[3]
+```
+
+![Costco 10Q filing](https://raw.githubusercontent.com/dgunning/edgartools/main/images/costco_10Q.jpg)
+
+### View the filing homepage
+You can view the filing homepage in the terminal using `filing.homepage`
+
+This gives you access to the `FilingHomepage` class that you can use to list all the documents
+and datafiles on the filing.
+
+```python
+filing.homepage
+```
+![Filing homapage](https://raw.githubusercontent.com/dgunning/edgartools/main/images/filing_homepage.jpg)
+
+### Open a filing
+
+You can open the filing in your browser using `filing.open()`. This will work on environments with access to the browser, 
+will probably not work on a remote server.
+```python
+filing.open()
+```
+
+### Open the Filing Homepage
+You can open the filing homepage in the browser using `filing.homepage.open()`.
+```python
+filing.homepage.open()
+```
+
+### Working with XBRL filings
+
+Some filings are in **XBRL (eXtensible Business Markup Language)** format. 
+These are mainly the newer filings, as the SEC has started requiring this for newer filings.
+
+If a filing is in XBRL format then it opens up a lot more ways to get structured data about that specific filing and also 
+about the company referred to in that filing.
+
+The `Filing` class has an `xbrl` function that will download, parse and structure the filing's XBRL document if one exists.
+If it does not exist, then `filing.xbrl()` will return `None`.
+
+The function `filing.xbrl()` returns a `FilingXbrl` instance, which wraps the data, and provides convenient
+ways of working with the xbrl data.
+
+
+```python
+filing_xbrl = filing.xbrl()
+```
+
+![Filing homapage](https://raw.githubusercontent.com/dgunning/edgartools/main/images/10Q_xbrl.jpg)
+
+
+#### Use DuckDB to query the filings
+
+A conveient way to query the filings data is to use **DuckDB**. If you call the `to_duckdb` function, you get an in-memory
+DuckDB database instance, with the filings registered as a table called `filings`.
+Then you can work directy with the DuckDB database, and run SQL against the filings data.
+
+In this example, we filter filings for **S-1** form types.
+
+```python
+db = filings.to_duckdb()
+# a duckdb.DuckDBPyConnection
+
+# Query the filings for S-1 filings and return a dataframe
+db.execute("""
+select * from filings where Form == 'S-1'
+""").df()
+```
 
 
 ## Using the Company API
 
 With the company API you find a company using the **cik** or **ticker**. 
 From the company you can access all their historical **filings**,
 and a dataset of the company **facts**.
@@ -143,15 +351,15 @@
 The **cik** is the id that uniquely identifies a company at the SEC.
 It is a number, but is sometimes shown in SEC Edgar resources as a string padded with leading zero's.
 For the edgar client API, just use the numbers and omit the leading zeroes.
 
 ```python
 company = Company(1324424)
 ```
-![expe](https://raw.githubusercontent.com/dgunning/edgartools/main/expe.png)
+![expe](https://raw.githubusercontent.com/dgunning/edgartools/main/images/expe.png)
 
 
 
 ### Find a company using ticker
 
 You can get a company using a ticker e.g. **SNOW**. This will do a lookup for the company cik using the ticker, then load the company using the cik.
 This makes it two calls versus one for the cik company lookup, but is sometimes more convenient since tickers are easier to remember that ciks.
@@ -161,15 +369,15 @@
 
 The ticker is case-insensitive so you can use `Company("snow")`
 or `Company("SNOW")`
 ```python
 snow = Company("snow")
 ```
 
-![snow inspect](https://raw.githubusercontent.com/dgunning/edgartools/main/snow-inspect.png)
+![snow inspect](https://raw.githubusercontent.com/dgunning/edgartools/main/images/snow-inspect.png)
 ### 
 
 
 ```python
 Company(1832950)
 ```
 
@@ -271,173 +479,14 @@
     df = db.execute("""
     select * from facts
     """).df()
 ```
 
 
 
-## Working with a Filing
-
-Once you have a filing you can do many things with it including getting the html text of the filing, get xbrl or xml, or list all the files in the filing.
-
-### Getting the html text of a filing
-
-```python
-html = filing.html()
-```
-
-
-To get the html text of the filing call `filing.html()`
-
-### Get the Homepage Url
-
-`filing.homepage_url` returns the homepage url of the filing. This is the main index page which lists
-all the files attached in the filing
-
-### Get the filing homepage
-
-To get access to all the documents on the filing you would call `filing.get_homepage()`.
-This gives you access to the `FilingHomepage` class that you can use to list all the documents
-and datafiles on the filing.
-
-
-### Working with XBRL filings
-
-Some filings are in **XBRL (eXtensible Business Markup Language)** format. 
-These are mainly the newer filings, as the SEC has started requiring this for newer filings.
-
-If a filing is in XBRL format then it opens up a lot more ways to get structured data about that specific filing and also 
-about the company referred to in that filing.
-
-The `Filing` class has an `xbrl` function that will download, parse and structure the filing's XBRL document if one exists.
-If it does not exist, then `filing.xbrl()` will return `None`.
-
-The function `filing.xbrl()` returns a `FilingXbrl` instance, which wraps the data, and provides convenient
-ways of working with the xbrl data.
-
-
-```python
-filing_xbrl = filing.xbrl()
-```
-
-## Using the Filings API
-
-The **Filings API** allows you to get the Edgar filing indexes published by the SEC.
-You would use it to get a bulk dataset of SEC filings for a given time period. With this dataset, you could filter by form type, by date or by company, 
-though if you intend to filter by a singe company, you should use the Company API.
-
-### The get_filings function
-The main way to use the Filings API is by `get_filings`
-
-`get_filings` accepts the following parameters
-- **year** a year `2015`, a List of years `[2013, 2015]` or a `range(2013, 2016)` 
-- **quarter** a quarter `2`, a List of quarters `[1,2,3]` or a `range(1,3)` 
-- **index** this is the type of index. By default it is `"form"`. If you want only XBRL filings use `"xbrl"`. 
-You can also use `"company"` but this will give you the same dataset as `"form"`, sorted by company instead of by form
-
-#### Get filings for 2021
-
-```python
-filings = get_filings(2021)
-```
-
-![Filings in 2021](https://raw.githubusercontent.com/dgunning/edgartools/main/filings_2021.jpg)
-
-#### Get filings for 2021 quarter 4
-Instead of getting the filings for an entire year, you can get the filings for a quarter.
-```python
-filings = get_filings(2021, 4)
-```
-
-#### Get filings between 2010 and 2019
-You can get the filings for a range of years, since the `year` parameter accepts a value, a list or a range.
-```python
-filings = get_filings(range(2010, 2020))
-```
-
-#### Get XBRL filings for 2022
-```python
-filings = get_filings(2022, index="xbrl")
-```
-
-
-#### Filtering Filings by form
-You can filter by form type by providing a form or list of forms.
-```python
-filings = get_filings(2022, form="10-K")
-
-# Filter by list of forms
-filings = get_filings(2022, form=["10-K", "10-Q"])
-```
-
-This will include form amendments e.g. "10-K/A" and "10-Q/A". To not include these set `amendments=False`
-```python
-# Filter by list of forms not including amendments
-filings = get_filings(2022, form=["10-K", "10-Q"], amendments=False)
-```
-
-### The Filings class
-
-The `get_filings` returns a `Filings` class, which wraps the data returned and provide convenient ways for working with filings.
-
-#### Convert the filings to a pandas dataframe
-
-The filings data is stored in the `Filings` class as a `pyarrow.Table`. You can get the data as a pandas dataframe using
-`to_pandas`
-```python
-df = filings.to_pandas()
-```
-
-## Working with an individual Filing
-
-Once you have retrieved Filings you can access individual filings using the bracket `[]` notation.
-```python
-filings = get_filings(2021)
-filing = filings[0]
-```
-![Filings in 2021](https://raw.githubusercontent.com/dgunning/edgartools/main/filings_2021.jpg)
-Pay attention to the index value displayed for the filings. This is the value you 
-will use to get the individual filing.
-```python
-filing = filings[0]
-```
-![A single filing](https://raw.githubusercontent.com/dgunning/edgartools/main/single_filing.png)
-
-### Open a filing
-
-You can open the filing in your browser using `filing.open()`
-```python
-filing.open()
-```
-
-### Open the Filing Homepage
-You can open the filing homepage in the browser using `filing.open_homepage()`
-```python
-filing.open()
-```
-
-
-#### Use DuckDB to query the filings
-
-A conveient way to query the filings data is to use **DuckDB**. If you call the `to_duckdb` function, you get an in-memory
-DuckDB database instance, with the filings registered as a table called `filings`.
-Then you can work directy with the DuckDB database, and run SQL against the filings data.
-
-In this example, we filter filings for **S-1** form types.
-
-```python
-db = filings.to_duckdb()
-# a duckdb.DuckDBPyConnection
-
-# Query the filings for S-1 filings and return a dataframe
-db.execute("""
-select * from filings where Form == 'S-1'
-""").df()
-```
-
 # Contributing
 
 Contributions are welcome! We would love to hear your thoughts on how this library could be better at working with SEC Edgar.
 
 ## Reporting Issues
 We use GitHub issues to track public bugs. 
 Report a bug by [opening a new issue](https://github.com/dgunning/edgartools/issues); it's that easy!
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
  ![edgar-tools-logo](https://raw.githubusercontent.com/dgunning/edgartools/
-main/edgar-tools.png) [![PyPI - Version](https://img.shields.io/pypi/v/
+main/images/edgar-tools.png) [![PyPI - Version](https://img.shields.io/pypi/v/
 edgartools.svg)](https://pypi.org/project/edgartools) ![GitHub last commit]
 (https://img.shields.io/github/last-commit/dgunning/edgartools) ![GitHub
 Workflow Status](https://img.shields.io/github/actions/workflow/status/
 dgunning/edgartools/python-hatch-workflow.yml) [![CodeFactor](https://
 www.codefactor.io/repository/github/dgunning/edgartools/badge)](https://
 www.codefactor.io/repository/github/dgunning/edgartools) [![Hatch project]
 (https://img.shields.io/badge/%F0%9F%A5%9A-Hatch-4051b5.svg)](https://
@@ -11,41 +11,42 @@
 dgunning/edgartools) -----   Table of Contents
    1. About_The_Project
           o Demo
           o Features
    2. Installation
    3. Usage
           o Setting_your_Edgar_user_identity
+          o Getting_Filings
           o Using_the_Company_API
-          o Using_the_Filings_API
    4. Contributing
    5. License
    6. Contact
- # About the project **`edgartools`** is a library for working Edgar filings in
-analytic workflows. ## Demo #### Get the Common Shares Issued amount from
-Snowflake's latest 10-Q filing ```python (Company("SNOW") .get_filings
-(form="10-Q") .latest() .xbrl() .to_duckdb().execute( """select fact, value,
-units, end_date from facts where fact = 'CommonStockSharesIssued' order by
-end_date desc limit 1 """ ).df() ) ``` ![Common Shares Issued](https://
-raw.githubusercontent.com/dgunning/edgartools/main/common-shares-issued.png)
-This example shows what can be done with **edgartools**. Under the hood the
-code does the following 1. Use the ticker **"SNOW"** to get the company's cik
-from the [Company Tickers JSON](https://www.sec.gov/file/company-tickers) 2.
-From the **cik** get the company's filings from the submissions endpoint
-`https://data.sec.gov/submissions/CIK{cik:010}.json` 3. Select the latest 10-
-Q filing 4. Download the XBRL file for that filing 5. Convert the XBRL data
-into a pandas dataframe 6. Register the dataframe as a DuckDB table 7. Execute
-the SQL and convert to a dataframe You might not want to chain the operations
-like this, and strictly speaking it might not be the most efficient, given how
-much work happens within those lines of code. This guide will show you step by
-step how to easily get SEC filing data and text into your analytic workflows.
-## Features - Download listings of Edgar filing by year, quarter since 1994 -
-Select an individual filing and download the html, XML or content of any
-attached file - View a filing XBRL as a dataframe and query it with SQL -
-Search for company by ticker or CIK - Get a company's filings - Get a dataset
+ # About the project **`edgartools`** is a library for working with SEC Edgar
+filings. You can query, filter and select any filing since 1994 and view the
+filing's html, text, xml or structured data. ## Demo #### Get the Common Shares
+Issued amount from Snowflake's latest 10-Q filing ```python (Company("SNOW")
+.get_filings(form="10-Q") .latest() .xbrl() .to_duckdb().execute( """select
+fact, value, units, end_date from facts where fact = 'CommonStockSharesIssued'
+order by end_date desc limit 1 """ ).df() ) ``` ![Common Shares Issued](https:/
+/raw.githubusercontent.com/dgunning/edgartools/main/images/common-shares-
+issued.png) This example shows what can be done with **edgartools**. Under the
+hood the code does the following 1. Use the ticker **"SNOW"** to get the
+company's cik from the [Company Tickers JSON](https://www.sec.gov/file/company-
+tickers) 2. From the **cik** get the company's filings from the submissions
+endpoint `https://data.sec.gov/submissions/CIK{cik:010}.json` 3. Select the
+latest 10-Q filing 4. Download the XBRL file for that filing 5. Convert the
+XBRL data into a pandas dataframe 6. Register the dataframe as a DuckDB table
+7. Execute the SQL and convert to a dataframe You might not want to chain the
+operations like this, and strictly speaking it might not be the most efficient,
+given how much work happens within those lines of code. This guide will show
+you step by step how to easily get SEC filing data and text into your analytic
+workflows. ## Features - Download listings of Edgar filing by year, quarter
+since 1994 - Select an individual filing and download the html, XML or content
+of any attached file - View a filing XBRL as a dataframe and query it with SQL
+- Search for company by ticker or CIK - Get a company's filings - Get a dataset
 of company's **facts** e.g. **CommonSharesOutstanding** - Query a company's
 facts as SQL using an in-memory **DuckDB** database # Installation ```console
 pip install edgartools ``` # Usage ## Set your Edgar user identity Before you
 can access the SEC Edgar API you need to set the identity that you will use to
 access Edgar. This is usually your name and email, or a company name and email.
 ```bash Sample Company Name AdminContact@.com ``` The user identity is sent in
 the User-Agent string and the Edgar API will refuse to respond to your request
@@ -53,37 +54,120 @@
 `EDGAR_IDENTITY` and use that in each request. So, you need to set this
 environment variable before using it. ### Setting EDGAR_IDENTITY in Linux/Mac
 ```bash export EDGAR_IDENTITY="Michael Mccallum mcalum@gmail.com" ``` ###
 Setting EDGAR_IDENTITY in Windows Powershell ```bash $Env:
 EDGAR_IDENTITY="Michael Mccallum mcalum@gmail.com" ``` Alternatively, you can
 call `set_identity` which does the same thing. ```python from edgar import
 set_identity set_identity("Michael Mccallum mcalum@gmail.com") ``` For more
-detail see https://www.sec.gov/os/accessing-edgar-data ## Using the Company API
-With the company API you find a company using the **cik** or **ticker**. From
-the company you can access all their historical **filings**, and a dataset of
-the company **facts**. The SEC's company API also supplies a lot more details
-about a company including industry, the SEC filer type, the mailing and
-business address and much more. ### Find a company using the cik The **cik** is
-the id that uniquely identifies a company at the SEC. It is a number, but is
-sometimes shown in SEC Edgar resources as a string padded with leading zero's.
-For the edgar client API, just use the numbers and omit the leading zeroes.
-```python company = Company(1324424) ``` ![expe](https://
-raw.githubusercontent.com/dgunning/edgartools/main/expe.png) ### Find a company
-using ticker You can get a company using a ticker e.g. **SNOW**. This will do a
-lookup for the company cik using the ticker, then load the company using the
-cik. This makes it two calls versus one for the cik company lookup, but is
-sometimes more convenient since tickers are easier to remember that ciks. Note
-that some companies have multiple tickers, so you technically cannot get SEC
-filings for a ticker. You instead get the SEC filings for the company to which
-the ticker belongs. The ticker is case-insensitive so you can use `Company
-("snow")` or `Company("SNOW")` ```python snow = Company("snow") ``` ![snow
-inspect](https://raw.githubusercontent.com/dgunning/edgartools/main/snow-
-inspect.png) ### ```python Company(1832950) ``` ### Get filings for a company
-To get the company's filings use `get_filings()`. This gets all the company's
-filings that are available from the Edgar submissions endpoint. ```python
+detail see https://www.sec.gov/os/accessing-edgar-data ## Getting filings To
+get started import from edgar and use the `get_filings` function. ```python
+from edgar import * filings = get_filings() ``` This gets the list of filings
+for the current year and quarter into a `Filings` object. ![Get Filings](https:
+//raw.githubusercontent.com/dgunning/edgartools/main/images/get_filings.jpg) If
+you need a different date range you can specify a year or years and a quarter
+or quarters. These are valid ways to specify the date range or filter by form
+or by filing date. ```python >>> filings = get_filings(2021) # Get filings for
+2021 >>> filings = get_filings(2021, 4) # Get filings for 2021 Q4 >>> filings =
+get_filings(2021, [3,4]) # Get filings for 2021 Q3 and Q4 >>> filings =
+get_filings([2020, 2021]) # Get filings for 2020 and 2021 >>> filings =
+get_filings([2020, 2021], 4) # Get filings for Q4 of 2020 and 2021 >>> filings
+= get_filings(range(2010, 2021)) # Get filings between 2010 and 2021 - does not
+include 2021 >>> filings = get_filings(2021, 4, form="D") # Get filings for
+2021 Q4 for form D >>> filings = get_filings(2021, 4, filing_date="2021-10-01")
+# Get filings for 2021 Q4 on "2021-10-01" >>> filings = get_filings(2021, 4,
+filing_date="2021-10-01:2021-10-10") # Get filings for 2021 Q4 between # "2021-
+10-01" and "2021-10-10" ``` ### Convert the filings to a pandas dataframe The
+filings data is stored in the `Filings` class as a `pyarrow.Table`. You can get
+the data as a pandas dataframe using `to_pandas` ```python df =
+filings.to_pandas() ``` ## Navigating filings The Filings object allows you to
+navigate through filings using `filings.next()` and `filings.prev()`. This
+shows you pages of the data - the page size is about 50. ```python # To see the
+next page of data filings.next() # To see the previous page filings.prev() # To
+see the current page filings.current() ``` ![Get next filings](https://
+raw.githubusercontent.com/dgunning/edgartools/main/images/filings_next.jpg) ##
+Getting the latest filings You can get the latest **n** filings by filing_date
+from a filings using `filings.latest()`. If you provide the parameter `n` it
+will return the latest `n` filings. ```python filing = filings.latest(n=5)
+filing ``` ![Latest filings](https://raw.githubusercontent.com/dgunning/
+edgartools/main/images/latest_filings.jpg) If you omit this parameter, or set
+`n=1` it will return a single `Filings object. ```python filing =
+filings.latest() filing ``` ![Latest filing](https://raw.githubusercontent.com/
+dgunning/edgartools/main/images/latest_filing.jpg) ## Filtering filings You can
+filter the filings object using te `filter()` function. This allows you to
+filter by filing date, or by form. ### Filtering filings by date To filter by
+filing date specify the filing date in **YYYY-MM-DD** format e.g. **2022-01-
+24** (Note the parameters `date` and `filing_date` are equivalent aliases for
+each other) ```python filings.filter(date="2021-01-24") # or filings.filter
+(filing_date="2021-01-24") ``` You can specify a filing date range using the
+colon ```python filings.filter(date="2021-01-12:2021-02-28") ``` To filter by
+dates before a specified date use `:YYYY-MM-DD' ```python filings.filter
+(date=":2021-02-28") ``` To filter by dates after a specified date use `YYYY-
+MM-DD:' ```python filings.filter(date="2021-02-28:") ``` ### Filtering filings
+by form You can filter filings by form using the `form` parameter. ```python
+filings.filter(form="10-K") ``` To filter by form e.g. **10-K** and include
+form amendments use `amendments = True`. ```python filings.filter(form="10-K",
+amendments=True) ``` ![Filter with amendments](https://
+raw.githubusercontent.com/dgunning/edgartools/main/images/
+filter_amendments.jpg) ## Getting a single filing You can get a single filing
+from the filings using the bracket operator `[]`, specifying the index of the
+filing. The index is the value displayed in the leftmost position in the
+filings table. For example, to get the **10-Q** for **Costco** in the table
+above use `filings[3]` ```python filing = filings[3] ``` ![Costco 10Q filing]
+(https://raw.githubusercontent.com/dgunning/edgartools/main/images/
+costco_10Q.jpg) ### View the filing homepage You can view the filing homepage
+in the terminal using `filing.homepage` This gives you access to the
+`FilingHomepage` class that you can use to list all the documents and datafiles
+on the filing. ```python filing.homepage ``` ![Filing homapage](https://
+raw.githubusercontent.com/dgunning/edgartools/main/images/filing_homepage.jpg)
+### Open a filing You can open the filing in your browser using `filing.open
+()`. This will work on environments with access to the browser, will probably
+not work on a remote server. ```python filing.open() ``` ### Open the Filing
+Homepage You can open the filing homepage in the browser using
+`filing.homepage.open()`. ```python filing.homepage.open() ``` ### Working with
+XBRL filings Some filings are in **XBRL (eXtensible Business Markup Language)**
+format. These are mainly the newer filings, as the SEC has started requiring
+this for newer filings. If a filing is in XBRL format then it opens up a lot
+more ways to get structured data about that specific filing and also about the
+company referred to in that filing. The `Filing` class has an `xbrl` function
+that will download, parse and structure the filing's XBRL document if one
+exists. If it does not exist, then `filing.xbrl()` will return `None`. The
+function `filing.xbrl()` returns a `FilingXbrl` instance, which wraps the data,
+and provides convenient ways of working with the xbrl data. ```python
+filing_xbrl = filing.xbrl() ``` ![Filing homapage](https://
+raw.githubusercontent.com/dgunning/edgartools/main/images/10Q_xbrl.jpg) ####
+Use DuckDB to query the filings A conveient way to query the filings data is to
+use **DuckDB**. If you call the `to_duckdb` function, you get an in-memory
+DuckDB database instance, with the filings registered as a table called
+`filings`. Then you can work directy with the DuckDB database, and run SQL
+against the filings data. In this example, we filter filings for **S-1** form
+types. ```python db = filings.to_duckdb() # a duckdb.DuckDBPyConnection # Query
+the filings for S-1 filings and return a dataframe db.execute(""" select * from
+filings where Form == 'S-1' """).df() ``` ## Using the Company API With the
+company API you find a company using the **cik** or **ticker**. From the
+company you can access all their historical **filings**, and a dataset of the
+company **facts**. The SEC's company API also supplies a lot more details about
+a company including industry, the SEC filer type, the mailing and business
+address and much more. ### Find a company using the cik The **cik** is the id
+that uniquely identifies a company at the SEC. It is a number, but is sometimes
+shown in SEC Edgar resources as a string padded with leading zero's. For the
+edgar client API, just use the numbers and omit the leading zeroes. ```python
+company = Company(1324424) ``` ![expe](https://raw.githubusercontent.com/
+dgunning/edgartools/main/images/expe.png) ### Find a company using ticker You
+can get a company using a ticker e.g. **SNOW**. This will do a lookup for the
+company cik using the ticker, then load the company using the cik. This makes
+it two calls versus one for the cik company lookup, but is sometimes more
+convenient since tickers are easier to remember that ciks. Note that some
+companies have multiple tickers, so you technically cannot get SEC filings for
+a ticker. You instead get the SEC filings for the company to which the ticker
+belongs. The ticker is case-insensitive so you can use `Company("snow")` or
+`Company("SNOW")` ```python snow = Company("snow") ``` ![snow inspect](https://
+raw.githubusercontent.com/dgunning/edgartools/main/images/snow-inspect.png) ###
+```python Company(1832950) ``` ### Get filings for a company To get the
+company's filings use `get_filings()`. This gets all the company's filings that
+are available from the Edgar submissions endpoint. ```python
 company.get_filings() ``` ### Filtering filings You can filter the company
 filings using a number of different parameters. ```python class CompanyFilings:
 ... def get_filings(self, *, form: str | List = None, accession_number: str |
 List = None, file_number: str | List = None, is_xbrl: bool = None,
 is_inline_xbrl: bool = None ): """ Get the company's filings and optionally
 filter by multiple criteria :param form: The form as a string e.g. '10-K' or
 List of strings ['10-Q', '10-K'] :param accession_number: The accession number
@@ -115,85 +199,17 @@
 data use the `facts` property. You can get the facts as a pandas dataframe by
 calling `to_pandas` ```python df = company_facts.to_pandas() ``` Facts differ
 among companies. To see what facts are available you can use the `facts_meta`
 property. #### Getting the facts as a DuckDB table Ypu can convert the facts to
 a DuckDB database which allows you to query the facts using SQL. ```python
 company_facts: CompanyFacts = get_company_facts(1318605) db =
 company_facts.to_duckdb() df = db.execute(""" select * from facts """).df() ```
-## Working with a Filing Once you have a filing you can do many things with it
-including getting the html text of the filing, get xbrl or xml, or list all the
-files in the filing. ### Getting the html text of a filing ```python html =
-filing.html() ``` To get the html text of the filing call `filing.html()` ###
-Get the Homepage Url `filing.homepage_url` returns the homepage url of the
-filing. This is the main index page which lists all the files attached in the
-filing ### Get the filing homepage To get access to all the documents on the
-filing you would call `filing.get_homepage()`. This gives you access to the
-`FilingHomepage` class that you can use to list all the documents and datafiles
-on the filing. ### Working with XBRL filings Some filings are in **XBRL
-(eXtensible Business Markup Language)** format. These are mainly the newer
-filings, as the SEC has started requiring this for newer filings. If a filing
-is in XBRL format then it opens up a lot more ways to get structured data about
-that specific filing and also about the company referred to in that filing. The
-`Filing` class has an `xbrl` function that will download, parse and structure
-the filing's XBRL document if one exists. If it does not exist, then
-`filing.xbrl()` will return `None`. The function `filing.xbrl()` returns a
-`FilingXbrl` instance, which wraps the data, and provides convenient ways of
-working with the xbrl data. ```python filing_xbrl = filing.xbrl() ``` ## Using
-the Filings API The **Filings API** allows you to get the Edgar filing indexes
-published by the SEC. You would use it to get a bulk dataset of SEC filings for
-a given time period. With this dataset, you could filter by form type, by date
-or by company, though if you intend to filter by a singe company, you should
-use the Company API. ### The get_filings function The main way to use the
-Filings API is by `get_filings` `get_filings` accepts the following parameters
-- **year** a year `2015`, a List of years `[2013, 2015]` or a `range(2013,
-2016)` - **quarter** a quarter `2`, a List of quarters `[1,2,3]` or a `range
-(1,3)` - **index** this is the type of index. By default it is `"form"`. If you
-want only XBRL filings use `"xbrl"`. You can also use `"company"` but this will
-give you the same dataset as `"form"`, sorted by company instead of by form
-#### Get filings for 2021 ```python filings = get_filings(2021) ``` ![Filings
-in 2021](https://raw.githubusercontent.com/dgunning/edgartools/main/
-filings_2021.jpg) #### Get filings for 2021 quarter 4 Instead of getting the
-filings for an entire year, you can get the filings for a quarter. ```python
-filings = get_filings(2021, 4) ``` #### Get filings between 2010 and 2019 You
-can get the filings for a range of years, since the `year` parameter accepts a
-value, a list or a range. ```python filings = get_filings(range(2010, 2020))
-``` #### Get XBRL filings for 2022 ```python filings = get_filings(2022,
-index="xbrl") ``` #### Filtering Filings by form You can filter by form type by
-providing a form or list of forms. ```python filings = get_filings(2022,
-form="10-K") # Filter by list of forms filings = get_filings(2022, form=["10-
-K", "10-Q"]) ``` This will include form amendments e.g. "10-K/A" and "10-Q/A".
-To not include these set `amendments=False` ```python # Filter by list of forms
-not including amendments filings = get_filings(2022, form=["10-K", "10-Q"],
-amendments=False) ``` ### The Filings class The `get_filings` returns a
-`Filings` class, which wraps the data returned and provide convenient ways for
-working with filings. #### Convert the filings to a pandas dataframe The
-filings data is stored in the `Filings` class as a `pyarrow.Table`. You can get
-the data as a pandas dataframe using `to_pandas` ```python df =
-filings.to_pandas() ``` ## Working with an individual Filing Once you have
-retrieved Filings you can access individual filings using the bracket `[]`
-notation. ```python filings = get_filings(2021) filing = filings[0] ``` !
-[Filings in 2021](https://raw.githubusercontent.com/dgunning/edgartools/main/
-filings_2021.jpg) Pay attention to the index value displayed for the filings.
-This is the value you will use to get the individual filing. ```python filing =
-filings[0] ``` ![A single filing](https://raw.githubusercontent.com/dgunning/
-edgartools/main/single_filing.png) ### Open a filing You can open the filing in
-your browser using `filing.open()` ```python filing.open() ``` ### Open the
-Filing Homepage You can open the filing homepage in the browser using
-`filing.open_homepage()` ```python filing.open() ``` #### Use DuckDB to query
-the filings A conveient way to query the filings data is to use **DuckDB**. If
-you call the `to_duckdb` function, you get an in-memory DuckDB database
-instance, with the filings registered as a table called `filings`. Then you can
-work directy with the DuckDB database, and run SQL against the filings data. In
-this example, we filter filings for **S-1** form types. ```python db =
-filings.to_duckdb() # a duckdb.DuckDBPyConnection # Query the filings for S-
-1 filings and return a dataframe db.execute(""" select * from filings where
-Form == 'S-1' """).df() ``` # Contributing Contributions are welcome! We would
-love to hear your thoughts on how this library could be better at working with
-SEC Edgar. ## Reporting Issues We use GitHub issues to track public bugs.
-Report a bug by [opening a new issue](https://github.com/dgunning/edgartools/
-issues); it's that easy! ## Making code changes - Fork the repo and create your
-branch from master. - If you've added code that should be tested, add tests. -
-If you've changed APIs, update the documentation. - Ensure the test suite
-passes. - Make sure your code lints. - Issue that pull request! # License
-`edgartools` is distributed under the terms of the [MIT](https://spdx.org/
-licenses/MIT.html) license. ## Contact [LinkedIn](https://www.linkedin.com/in/
-dwight-gunning-860124/)
+# Contributing Contributions are welcome! We would love to hear your thoughts
+on how this library could be better at working with SEC Edgar. ## Reporting
+Issues We use GitHub issues to track public bugs. Report a bug by [opening a
+new issue](https://github.com/dgunning/edgartools/issues); it's that easy! ##
+Making code changes - Fork the repo and create your branch from master. - If
+you've added code that should be tested, add tests. - If you've changed APIs,
+update the documentation. - Ensure the test suite passes. - Make sure your code
+lints. - Issue that pull request! # License `edgartools` is distributed under
+the terms of the [MIT](https://spdx.org/licenses/MIT.html) license. ## Contact
+[LinkedIn](https://www.linkedin.com/in/dwight-gunning-860124/)
```

### Comparing `edgartools-1.8.0/pyproject.toml` & `edgartools-1.9.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `edgartools-1.8.0/PKG-INFO` & `edgartools-1.9.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 6564 6761  : 2.1.Name: edga
 00000020: 7274 6f6f 6c73 0a56 6572 7369 6f6e 3a20  rtools.Version: 
-00000030: 312e 382e 300a 5375 6d6d 6172 793a 204f  1.8.0.Summary: O
+00000030: 312e 392e 300a 5375 6d6d 6172 793a 204f  1.9.0.Summary: O
 00000040: 6e65 206f 6620 7468 6520 6e69 6365 7374  ne of the nicest
 00000050: 206c 6f6f 6b69 6e67 2045 4447 4152 206c   looking EDGAR l
 00000060: 6962 7261 7269 6573 206f 7574 2074 6865  ibraries out the
 00000070: 7265 0a50 726f 6a65 6374 2d55 524c 3a20  re.Project-URL: 
 00000080: 446f 6375 6d65 6e74 6174 696f 6e2c 2068  Documentation, h
 00000090: 7474 7073 3a2f 2f64 6775 6e6e 696e 672e  ttps://dgunning.
 000000a0: 6769 7468 7562 2e69 6f2f 6564 6761 7274  github.io/edgart
@@ -80,975 +80,1061 @@
 000004f0: 696f 6e2d 436f 6e74 656e 742d 5479 7065  ion-Content-Type
 00000500: 3a20 7465 7874 2f6d 6172 6b64 6f77 6e0a  : text/markdown.
 00000510: 0a0a 0a21 5b65 6467 6172 2d74 6f6f 6c73  ...![edgar-tools
 00000520: 2d6c 6f67 6f5d 2868 7474 7073 3a2f 2f72  -logo](https://r
 00000530: 6177 2e67 6974 6875 6275 7365 7263 6f6e  aw.githubusercon
 00000540: 7465 6e74 2e63 6f6d 2f64 6775 6e6e 696e  tent.com/dgunnin
 00000550: 672f 6564 6761 7274 6f6f 6c73 2f6d 6169  g/edgartools/mai
-00000560: 6e2f 6564 6761 722d 746f 6f6c 732e 706e  n/edgar-tools.pn
-00000570: 6729 0a0a 5b21 5b50 7950 4920 2d20 5665  g)..[![PyPI - Ve
-00000580: 7273 696f 6e5d 2868 7474 7073 3a2f 2f69  rsion](https://i
-00000590: 6d67 2e73 6869 656c 6473 2e69 6f2f 7079  mg.shields.io/py
-000005a0: 7069 2f76 2f65 6467 6172 746f 6f6c 732e  pi/v/edgartools.
-000005b0: 7376 6729 5d28 6874 7470 733a 2f2f 7079  svg)](https://py
-000005c0: 7069 2e6f 7267 2f70 726f 6a65 6374 2f65  pi.org/project/e
-000005d0: 6467 6172 746f 6f6c 7329 0a21 5b47 6974  dgartools).![Git
-000005e0: 4875 6220 6c61 7374 2063 6f6d 6d69 745d  Hub last commit]
-000005f0: 2868 7474 7073 3a2f 2f69 6d67 2e73 6869  (https://img.shi
-00000600: 656c 6473 2e69 6f2f 6769 7468 7562 2f6c  elds.io/github/l
-00000610: 6173 742d 636f 6d6d 6974 2f64 6775 6e6e  ast-commit/dgunn
-00000620: 696e 672f 6564 6761 7274 6f6f 6c73 290a  ing/edgartools).
-00000630: 215b 4769 7448 7562 2057 6f72 6b66 6c6f  ![GitHub Workflo
-00000640: 7720 5374 6174 7573 5d28 6874 7470 733a  w Status](https:
-00000650: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
-00000660: 2f67 6974 6875 622f 6163 7469 6f6e 732f  /github/actions/
-00000670: 776f 726b 666c 6f77 2f73 7461 7475 732f  workflow/status/
-00000680: 6467 756e 6e69 6e67 2f65 6467 6172 746f  dgunning/edgarto
-00000690: 6f6c 732f 7079 7468 6f6e 2d68 6174 6368  ols/python-hatch
-000006a0: 2d77 6f72 6b66 6c6f 772e 796d 6c29 0a5b  -workflow.yml).[
-000006b0: 215b 436f 6465 4661 6374 6f72 5d28 6874  ![CodeFactor](ht
-000006c0: 7470 733a 2f2f 7777 772e 636f 6465 6661  tps://www.codefa
-000006d0: 6374 6f72 2e69 6f2f 7265 706f 7369 746f  ctor.io/reposito
-000006e0: 7279 2f67 6974 6875 622f 6467 756e 6e69  ry/github/dgunni
-000006f0: 6e67 2f65 6467 6172 746f 6f6c 732f 6261  ng/edgartools/ba
-00000700: 6467 6529 5d28 6874 7470 733a 2f2f 7777  dge)](https://ww
-00000710: 772e 636f 6465 6661 6374 6f72 2e69 6f2f  w.codefactor.io/
-00000720: 7265 706f 7369 746f 7279 2f67 6974 6875  repository/githu
-00000730: 622f 6467 756e 6e69 6e67 2f65 6467 6172  b/dgunning/edgar
-00000740: 746f 6f6c 7329 0a5b 215b 4861 7463 6820  tools).[![Hatch 
-00000750: 7072 6f6a 6563 745d 2868 7474 7073 3a2f  project](https:/
-00000760: 2f69 6d67 2e73 6869 656c 6473 2e69 6f2f  /img.shields.io/
-00000770: 6261 6467 652f 2546 3025 3946 2541 3525  badge/%F0%9F%A5%
-00000780: 3941 2d48 6174 6368 2d34 3035 3162 352e  9A-Hatch-4051b5.
-00000790: 7376 6729 5d28 6874 7470 733a 2f2f 6769  svg)](https://gi
-000007a0: 7468 7562 2e63 6f6d 2f70 7970 612f 6861  thub.com/pypa/ha
-000007b0: 7463 6829 0a21 5b47 6974 4875 625d 2868  tch).![GitHub](h
-000007c0: 7474 7073 3a2f 2f69 6d67 2e73 6869 656c  ttps://img.shiel
-000007d0: 6473 2e69 6f2f 6769 7468 7562 2f6c 6963  ds.io/github/lic
-000007e0: 656e 7365 2f64 6775 6e6e 696e 672f 6564  ense/dgunning/ed
-000007f0: 6761 7274 6f6f 6c73 290a 2d2d 2d2d 2d0a  gartools).-----.
-00000800: 0a3c 212d 2d20 5441 424c 4520 4f46 2043  .<!-- TABLE OF C
-00000810: 4f4e 5445 4e54 5320 2d2d 3e0a 3c64 6574  ONTENTS -->.<det
-00000820: 6169 6c73 3e0a 2020 3c73 756d 6d61 7279  ails>.  <summary
-00000830: 3e54 6162 6c65 206f 6620 436f 6e74 656e  >Table of Conten
-00000840: 7473 3c2f 7375 6d6d 6172 793e 0a20 203c  ts</summary>.  <
-00000850: 6f6c 3e0a 2020 2020 3c6c 693e 0a20 2020  ol>.    <li>.   
-00000860: 2020 203c 6120 6872 6566 3d22 2361 626f     <a href="#abo
-00000870: 7574 2d74 6865 2d70 726f 6a65 6374 223e  ut-the-project">
-00000880: 4162 6f75 7420 5468 6520 5072 6f6a 6563  About The Projec
-00000890: 743c 2f61 3e0a 2020 2020 2020 3c75 6c3e  t</a>.      <ul>
-000008a0: 0a20 2020 2020 2020 203c 6c69 3e3c 6120  .        <li><a 
-000008b0: 6872 6566 3d22 2364 656d 6f22 3e44 656d  href="#demo">Dem
-000008c0: 6f3c 2f61 3e3c 2f6c 693e 0a20 2020 2020  o</a></li>.     
-000008d0: 2020 203c 6c69 3e3c 6120 6872 6566 3d22     <li><a href="
-000008e0: 2366 6561 7475 7265 7322 3e46 6561 7475  #features">Featu
-000008f0: 7265 733c 2f61 3e3c 2f6c 693e 0a20 2020  res</a></li>.   
-00000900: 2020 203c 2f75 6c3e 0a20 2020 203c 2f6c     </ul>.    </l
-00000910: 693e 0a20 2020 203c 6c69 3e0a 2020 2020  i>.    <li>.    
-00000920: 2020 2020 3c61 2068 7265 663d 2223 696e      <a href="#in
-00000930: 7374 616c 6c61 7469 6f6e 223e 496e 7374  stallation">Inst
-00000940: 616c 6c61 7469 6f6e 3c2f 613e 0a20 2020  allation</a>.   
-00000950: 203c 2f6c 693e 0a20 2020 203c 6c69 3e0a   </li>.    <li>.
-00000960: 2020 2020 2020 2020 3c61 2068 7265 663d          <a href=
-00000970: 2223 7573 6167 6522 3e55 7361 6765 3c2f  "#usage">Usage</
-00000980: 613e 0a20 2020 2020 2020 203c 756c 3e0a  a>.        <ul>.
-00000990: 2020 2020 2020 2020 2020 2020 3c6c 693e              <li>
-000009a0: 3c61 2068 7265 663d 2223 7365 7474 696e  <a href="#settin
-000009b0: 672d 796f 7572 2d65 6467 6172 2d75 7365  g-your-edgar-use
-000009c0: 722d 6964 656e 7469 7479 223e 5365 7474  r-identity">Sett
-000009d0: 696e 6720 796f 7572 2045 6467 6172 2075  ing your Edgar u
-000009e0: 7365 7220 6964 656e 7469 7479 3c2f 613e  ser identity</a>
-000009f0: 3c2f 6c69 3e0a 2020 2020 2020 2020 2020  </li>.          
-00000a00: 2020 3c6c 693e 3c61 2068 7265 663d 2223    <li><a href="#
-00000a10: 7573 696e 672d 7468 652d 636f 6d70 616e  using-the-compan
-00000a20: 792d 6170 6922 3e55 7369 6e67 2074 6865  y-api">Using the
-00000a30: 2043 6f6d 7061 6e79 2041 5049 3c2f 613e   Company API</a>
-00000a40: 3c2f 6c69 3e0a 2020 2020 2020 2020 2020  </li>.          
-00000a50: 2020 3c6c 693e 3c61 2068 7265 663d 2223    <li><a href="#
-00000a60: 7573 696e 672d 7468 652d 6669 6c69 6e67  using-the-filing
-00000a70: 732d 6170 6922 3e55 7369 6e67 2074 6865  s-api">Using the
-00000a80: 2046 696c 696e 6773 2041 5049 3c2f 613e   Filings API</a>
-00000a90: 3c2f 6c69 3e0a 2020 2020 2020 3c2f 756c  </li>.      </ul
-00000aa0: 3e0a 2020 2020 3c2f 6c69 3e0a 2020 2020  >.    </li>.    
-00000ab0: 3c6c 693e 3c61 2068 7265 663d 2223 636f  <li><a href="#co
-00000ac0: 6e74 7269 6275 7469 6e67 223e 436f 6e74  ntributing">Cont
-00000ad0: 7269 6275 7469 6e67 3c2f 613e 3c2f 6c69  ributing</a></li
-00000ae0: 3e0a 2020 2020 3c6c 693e 3c61 2068 7265  >.    <li><a hre
-00000af0: 663d 2223 6c69 6365 6e73 6522 3e4c 6963  f="#license">Lic
-00000b00: 656e 7365 3c2f 613e 3c2f 6c69 3e0a 2020  ense</a></li>.  
-00000b10: 2020 3c6c 693e 3c61 2068 7265 663d 2223    <li><a href="#
-00000b20: 636f 6e74 6163 7422 3e43 6f6e 7461 6374  contact">Contact
-00000b30: 3c2f 613e 3c2f 6c69 3e0a 2020 3c2f 6f6c  </a></li>.  </ol
-00000b40: 3e0a 3c2f 6465 7461 696c 733e 0a0a 2320  >.</details>..# 
-00000b50: 4162 6f75 7420 7468 6520 7072 6f6a 6563  About the projec
-00000b60: 740a 0a2a 2a60 6564 6761 7274 6f6f 6c73  t..**`edgartools
-00000b70: 602a 2a20 6973 2061 206c 6962 7261 7279  `** is a library
-00000b80: 2066 6f72 2077 6f72 6b69 6e67 2045 6467   for working Edg
-00000b90: 6172 2066 696c 696e 6773 2069 6e20 616e  ar filings in an
-00000ba0: 616c 7974 6963 2077 6f72 6b66 6c6f 7773  alytic workflows
-00000bb0: 2e0a 0a23 2320 4465 6d6f 0a0a 2323 2323  ...## Demo..####
-00000bc0: 2047 6574 2074 6865 2043 6f6d 6d6f 6e20   Get the Common 
-00000bd0: 5368 6172 6573 2049 7373 7565 6420 616d  Shares Issued am
-00000be0: 6f75 6e74 2066 726f 6d20 536e 6f77 666c  ount from Snowfl
-00000bf0: 616b 6527 7320 6c61 7465 7374 2031 302d  ake's latest 10-
-00000c00: 5120 6669 6c69 6e67 0a0a 6060 6070 7974  Q filing..```pyt
-00000c10: 686f 6e0a 2843 6f6d 7061 6e79 2822 534e  hon.(Company("SN
-00000c20: 4f57 2229 0a20 2020 2020 2020 202e 6765  OW").        .ge
-00000c30: 745f 6669 6c69 6e67 7328 666f 726d 3d22  t_filings(form="
-00000c40: 3130 2d51 2229 0a20 2020 2020 2020 202e  10-Q").        .
-00000c50: 6c61 7465 7374 2829 0a20 2020 2020 2020  latest().       
-00000c60: 202e 7862 726c 2829 0a20 2020 2020 2020   .xbrl().       
-00000c70: 202e 746f 5f64 7563 6b64 6228 292e 6578   .to_duckdb().ex
-00000c80: 6563 7574 6528 0a20 2020 2020 2020 2022  ecute(.        "
-00000c90: 2222 7365 6c65 6374 2066 6163 742c 2076  ""select fact, v
-00000ca0: 616c 7565 2c20 756e 6974 732c 2065 6e64  alue, units, end
-00000cb0: 5f64 6174 6520 6672 6f6d 2066 6163 7473  _date from facts
-00000cc0: 200a 2020 2020 2020 2020 2020 2077 6865   .           whe
-00000cd0: 7265 2066 6163 7420 3d20 2743 6f6d 6d6f  re fact = 'Commo
-00000ce0: 6e53 746f 636b 5368 6172 6573 4973 7375  nStockSharesIssu
-00000cf0: 6564 2720 0a20 2020 2020 2020 2020 2020  ed' .           
-00000d00: 6f72 6465 7220 6279 2065 6e64 5f64 6174  order by end_dat
-00000d10: 6520 6465 7363 206c 696d 6974 2031 0a20  e desc limit 1. 
-00000d20: 2020 2020 2020 2022 2222 0a20 2020 2029         """.    )
-00000d30: 2e64 6628 290a 290a 6060 600a 0a21 5b43  .df().).```..![C
-00000d40: 6f6d 6d6f 6e20 5368 6172 6573 2049 7373  ommon Shares Iss
-00000d50: 7565 645d 2868 7474 7073 3a2f 2f72 6177  ued](https://raw
-00000d60: 2e67 6974 6875 6275 7365 7263 6f6e 7465  .githubuserconte
-00000d70: 6e74 2e63 6f6d 2f64 6775 6e6e 696e 672f  nt.com/dgunning/
-00000d80: 6564 6761 7274 6f6f 6c73 2f6d 6169 6e2f  edgartools/main/
-00000d90: 636f 6d6d 6f6e 2d73 6861 7265 732d 6973  common-shares-is
-00000da0: 7375 6564 2e70 6e67 290a 0a54 6869 7320  sued.png)..This 
-00000db0: 6578 616d 706c 6520 7368 6f77 7320 7768  example shows wh
-00000dc0: 6174 2063 616e 2062 6520 646f 6e65 2077  at can be done w
-00000dd0: 6974 6820 2a2a 6564 6761 7274 6f6f 6c73  ith **edgartools
-00000de0: 2a2a 2e0a 0a55 6e64 6572 2074 6865 2068  **...Under the h
-00000df0: 6f6f 6420 7468 6520 636f 6465 2064 6f65  ood the code doe
-00000e00: 7320 7468 6520 666f 6c6c 6f77 696e 670a  s the following.
-00000e10: 0a31 2e20 5573 6520 7468 6520 7469 636b  .1. Use the tick
-00000e20: 6572 202a 2a22 534e 4f57 222a 2a20 746f  er **"SNOW"** to
-00000e30: 2067 6574 2074 6865 2063 6f6d 7061 6e79   get the company
-00000e40: 2773 2063 696b 2066 726f 6d20 7468 6520  's cik from the 
-00000e50: 5b43 6f6d 7061 6e79 2054 6963 6b65 7273  [Company Tickers
-00000e60: 204a 534f 4e5d 2868 7474 7073 3a2f 2f77   JSON](https://w
-00000e70: 7777 2e73 6563 2e67 6f76 2f66 696c 652f  ww.sec.gov/file/
-00000e80: 636f 6d70 616e 792d 7469 636b 6572 7329  company-tickers)
-00000e90: 0a32 2e20 4672 6f6d 2074 6865 202a 2a63  .2. From the **c
-00000ea0: 696b 2a2a 2067 6574 2074 6865 2063 6f6d  ik** get the com
-00000eb0: 7061 6e79 2773 2066 696c 696e 6773 2066  pany's filings f
-00000ec0: 726f 6d20 7468 6520 7375 626d 6973 7369  rom the submissi
-00000ed0: 6f6e 7320 656e 6470 6f69 6e74 2060 6874  ons endpoint `ht
-00000ee0: 7470 733a 2f2f 6461 7461 2e73 6563 2e67  tps://data.sec.g
-00000ef0: 6f76 2f73 7562 6d69 7373 696f 6e73 2f43  ov/submissions/C
-00000f00: 494b 7b63 696b 3a30 3130 7d2e 6a73 6f6e  IK{cik:010}.json
-00000f10: 600a 332e 2053 656c 6563 7420 7468 6520  `.3. Select the 
-00000f20: 6c61 7465 7374 2031 302d 5120 6669 6c69  latest 10-Q fili
-00000f30: 6e67 0a34 2e20 446f 776e 6c6f 6164 2074  ng.4. Download t
-00000f40: 6865 2058 4252 4c20 6669 6c65 2066 6f72  he XBRL file for
-00000f50: 2074 6861 7420 6669 6c69 6e67 0a35 2e20   that filing.5. 
-00000f60: 436f 6e76 6572 7420 7468 6520 5842 524c  Convert the XBRL
-00000f70: 2064 6174 6120 696e 746f 2061 2070 616e   data into a pan
-00000f80: 6461 7320 6461 7461 6672 616d 650a 362e  das dataframe.6.
-00000f90: 2052 6567 6973 7465 7220 7468 6520 6461   Register the da
-00000fa0: 7461 6672 616d 6520 6173 2061 2044 7563  taframe as a Duc
-00000fb0: 6b44 4220 7461 626c 650a 372e 2045 7865  kDB table.7. Exe
-00000fc0: 6375 7465 2074 6865 2053 514c 2061 6e64  cute the SQL and
-00000fd0: 2063 6f6e 7665 7274 2074 6f20 6120 6461   convert to a da
-00000fe0: 7461 6672 616d 650a 0a59 6f75 206d 6967  taframe..You mig
-00000ff0: 6874 206e 6f74 2077 616e 7420 746f 2063  ht not want to c
-00001000: 6861 696e 2074 6865 206f 7065 7261 7469  hain the operati
-00001010: 6f6e 7320 6c69 6b65 2074 6869 732c 2061  ons like this, a
-00001020: 6e64 2073 7472 6963 746c 7920 7370 6561  nd strictly spea
-00001030: 6b69 6e67 2069 7420 6d69 6768 7420 6e6f  king it might no
-00001040: 7420 6265 2074 6865 206d 6f73 7420 6566  t be the most ef
-00001050: 6669 6369 656e 742c 200a 6769 7665 6e20  ficient, .given 
-00001060: 686f 7720 6d75 6368 2077 6f72 6b20 6861  how much work ha
-00001070: 7070 656e 7320 7769 7468 696e 2074 686f  ppens within tho
-00001080: 7365 206c 696e 6573 206f 6620 636f 6465  se lines of code
-00001090: 2e20 5468 6973 2067 7569 6465 2077 696c  . This guide wil
-000010a0: 6c20 7368 6f77 2079 6f75 2073 7465 7020  l show you step 
-000010b0: 6279 2073 7465 700a 686f 7720 746f 2065  by step.how to e
-000010c0: 6173 696c 7920 6765 7420 5345 4320 6669  asily get SEC fi
-000010d0: 6c69 6e67 2064 6174 6120 616e 6420 7465  ling data and te
-000010e0: 7874 2069 6e74 6f20 796f 7572 2061 6e61  xt into your ana
-000010f0: 6c79 7469 6320 776f 726b 666c 6f77 732e  lytic workflows.
-00001100: 0a0a 0a23 2320 4665 6174 7572 6573 0a0a  ...## Features..
-00001110: 2d20 446f 776e 6c6f 6164 206c 6973 7469  - Download listi
-00001120: 6e67 7320 6f66 2045 6467 6172 2066 696c  ngs of Edgar fil
-00001130: 696e 6720 6279 2079 6561 722c 2071 7561  ing by year, qua
-00001140: 7274 6572 2073 696e 6365 2031 3939 340a  rter since 1994.
-00001150: 2d20 5365 6c65 6374 2061 6e20 696e 6469  - Select an indi
-00001160: 7669 6475 616c 2066 696c 696e 6720 616e  vidual filing an
-00001170: 6420 646f 776e 6c6f 6164 2074 6865 2068  d download the h
-00001180: 746d 6c2c 2058 4d4c 206f 7220 636f 6e74  tml, XML or cont
-00001190: 656e 7420 6f66 2061 6e79 2061 7474 6163  ent of any attac
-000011a0: 6865 6420 6669 6c65 0a2d 2056 6965 7720  hed file.- View 
-000011b0: 6120 6669 6c69 6e67 2058 4252 4c20 6173  a filing XBRL as
-000011c0: 2061 2064 6174 6166 7261 6d65 2061 6e64   a dataframe and
-000011d0: 2071 7565 7279 2069 7420 7769 7468 2053   query it with S
-000011e0: 514c 0a2d 2053 6561 7263 6820 666f 7220  QL.- Search for 
-000011f0: 636f 6d70 616e 7920 6279 2074 6963 6b65  company by ticke
-00001200: 7220 6f72 2043 494b 0a2d 2047 6574 2061  r or CIK.- Get a
-00001210: 2063 6f6d 7061 6e79 2773 2066 696c 696e   company's filin
-00001220: 6773 200a 2d20 4765 7420 6120 6461 7461  gs .- Get a data
-00001230: 7365 7420 6f66 2063 6f6d 7061 6e79 2773  set of company's
-00001240: 202a 2a66 6163 7473 2a2a 2065 2e67 2e20   **facts** e.g. 
-00001250: 2a2a 436f 6d6d 6f6e 5368 6172 6573 4f75  **CommonSharesOu
-00001260: 7473 7461 6e64 696e 672a 2a0a 2d20 5175  tstanding**.- Qu
-00001270: 6572 7920 6120 636f 6d70 616e 7927 7320  ery a company's 
-00001280: 6661 6374 7320 6173 2053 514c 2075 7369  facts as SQL usi
-00001290: 6e67 2061 6e20 696e 2d6d 656d 6f72 7920  ng an in-memory 
-000012a0: 2a2a 4475 636b 4442 2a2a 2064 6174 6162  **DuckDB** datab
-000012b0: 6173 650a 0a23 2049 6e73 7461 6c6c 6174  ase..# Installat
-000012c0: 696f 6e0a 0a60 6060 636f 6e73 6f6c 650a  ion..```console.
-000012d0: 7069 7020 696e 7374 616c 6c20 6564 6761  pip install edga
-000012e0: 7274 6f6f 6c73 0a60 6060 0a0a 2320 5573  rtools.```..# Us
-000012f0: 6167 650a 0a0a 2323 2053 6574 2079 6f75  age...## Set you
-00001300: 7220 4564 6761 7220 7573 6572 2069 6465  r Edgar user ide
-00001310: 6e74 6974 790a 0a42 6566 6f72 6520 796f  ntity..Before yo
-00001320: 7520 6361 6e20 6163 6365 7373 2074 6865  u can access the
-00001330: 2053 4543 2045 6467 6172 2041 5049 2079   SEC Edgar API y
-00001340: 6f75 206e 6565 6420 746f 2073 6574 2074  ou need to set t
-00001350: 6865 2069 6465 6e74 6974 7920 7468 6174  he identity that
-00001360: 2079 6f75 2077 696c 6c20 7573 6520 746f   you will use to
-00001370: 2061 6363 6573 7320 4564 6761 722e 0a54   access Edgar..T
-00001380: 6869 7320 6973 2075 7375 616c 6c79 2079  his is usually y
-00001390: 6f75 7220 6e61 6d65 2061 6e64 2065 6d61  our name and ema
-000013a0: 696c 2c20 6f72 2061 2063 6f6d 7061 6e79  il, or a company
-000013b0: 206e 616d 6520 616e 6420 656d 6169 6c2e   name and email.
-000013c0: 0a60 6060 6261 7368 0a53 616d 706c 6520  .```bash.Sample 
-000013d0: 436f 6d70 616e 7920 4e61 6d65 2041 646d  Company Name Adm
-000013e0: 696e 436f 6e74 6163 7440 3c73 616d 706c  inContact@<sampl
-000013f0: 6520 636f 6d70 616e 7920 646f 6d61 696e  e company domain
-00001400: 3e2e 636f 6d0a 6060 600a 0a54 6865 2075  >.com.```..The u
-00001410: 7365 7220 6964 656e 7469 7479 2069 7320  ser identity is 
-00001420: 7365 6e74 2069 6e20 7468 6520 5573 6572  sent in the User
-00001430: 2d41 6765 6e74 2073 7472 696e 6720 616e  -Agent string an
-00001440: 6420 7468 6520 4564 6761 7220 4150 4920  d the Edgar API 
-00001450: 7769 6c6c 2072 6566 7573 6520 746f 2072  will refuse to r
-00001460: 6573 706f 6e64 2074 6f20 796f 7572 2072  espond to your r
-00001470: 6571 7565 7374 2077 6974 686f 7574 2069  equest without i
-00001480: 742e 0a0a 4564 6761 7254 6f6f 6c73 2077  t...EdgarTools w
-00001490: 696c 6c20 6c6f 6f6b 2066 6f72 2061 6e20  ill look for an 
-000014a0: 656e 7669 726f 6e6d 656e 7420 7661 7269  environment vari
-000014b0: 6162 6c65 2063 616c 6c65 6420 6045 4447  able called `EDG
-000014c0: 4152 5f49 4445 4e54 4954 5960 2061 6e64  AR_IDENTITY` and
-000014d0: 2075 7365 2074 6861 7420 696e 2065 6163   use that in eac
-000014e0: 6820 7265 7175 6573 742e 0a53 6f2c 2079  h request..So, y
-000014f0: 6f75 206e 6565 6420 746f 2073 6574 2074  ou need to set t
-00001500: 6869 7320 656e 7669 726f 6e6d 656e 7420  his environment 
-00001510: 7661 7269 6162 6c65 2062 6566 6f72 6520  variable before 
-00001520: 7573 696e 6720 6974 2e0a 0a23 2323 2053  using it...### S
-00001530: 6574 7469 6e67 2045 4447 4152 5f49 4445  etting EDGAR_IDE
-00001540: 4e54 4954 5920 696e 204c 696e 7578 2f4d  NTITY in Linux/M
-00001550: 6163 0a60 6060 6261 7368 0a65 7870 6f72  ac.```bash.expor
-00001560: 7420 4544 4741 525f 4944 454e 5449 5459  t EDGAR_IDENTITY
-00001570: 3d22 4d69 6368 6165 6c20 4d63 6361 6c6c  ="Michael Mccall
-00001580: 756d 206d 6361 6c75 6d40 676d 6169 6c2e  um mcalum@gmail.
-00001590: 636f 6d22 0a60 6060 0a0a 2323 2320 5365  com".```..### Se
-000015a0: 7474 696e 6720 4544 4741 525f 4944 454e  tting EDGAR_IDEN
-000015b0: 5449 5459 2069 6e20 5769 6e64 6f77 7320  TITY in Windows 
-000015c0: 506f 7765 7273 6865 6c6c 0a60 6060 6261  Powershell.```ba
-000015d0: 7368 0a20 2445 6e76 3a45 4447 4152 5f49  sh. $Env:EDGAR_I
-000015e0: 4445 4e54 4954 593d 224d 6963 6861 656c  DENTITY="Michael
-000015f0: 204d 6363 616c 6c75 6d20 6d63 616c 756d   Mccallum mcalum
-00001600: 4067 6d61 696c 2e63 6f6d 220a 6060 600a  @gmail.com".```.
-00001610: 416c 7465 726e 6174 6976 656c 792c 2079  Alternatively, y
-00001620: 6f75 2063 616e 2063 616c 6c20 6073 6574  ou can call `set
-00001630: 5f69 6465 6e74 6974 7960 2077 6869 6368  _identity` which
-00001640: 2064 6f65 7320 7468 6520 7361 6d65 2074   does the same t
-00001650: 6869 6e67 2e0a 0a60 6060 7079 7468 6f6e  hing...```python
-00001660: 0a66 726f 6d20 6564 6761 7220 696d 706f  .from edgar impo
-00001670: 7274 2073 6574 5f69 6465 6e74 6974 790a  rt set_identity.
-00001680: 7365 745f 6964 656e 7469 7479 2822 4d69  set_identity("Mi
-00001690: 6368 6165 6c20 4d63 6361 6c6c 756d 206d  chael Mccallum m
-000016a0: 6361 6c75 6d40 676d 6169 6c2e 636f 6d22  calum@gmail.com"
-000016b0: 290a 6060 600a 0a0a 466f 7220 6d6f 7265  ).```...For more
-000016c0: 2064 6574 6169 6c20 7365 6520 6874 7470   detail see http
-000016d0: 733a 2f2f 7777 772e 7365 632e 676f 762f  s://www.sec.gov/
-000016e0: 6f73 2f61 6363 6573 7369 6e67 2d65 6467  os/accessing-edg
-000016f0: 6172 2d64 6174 610a 0a0a 2323 2055 7369  ar-data...## Usi
-00001700: 6e67 2074 6865 2043 6f6d 7061 6e79 2041  ng the Company A
-00001710: 5049 0a0a 5769 7468 2074 6865 2063 6f6d  PI..With the com
-00001720: 7061 6e79 2041 5049 2079 6f75 2066 696e  pany API you fin
-00001730: 6420 6120 636f 6d70 616e 7920 7573 696e  d a company usin
-00001740: 6720 7468 6520 2a2a 6369 6b2a 2a20 6f72  g the **cik** or
-00001750: 202a 2a74 6963 6b65 722a 2a2e 200a 4672   **ticker**. .Fr
-00001760: 6f6d 2074 6865 2063 6f6d 7061 6e79 2079  om the company y
-00001770: 6f75 2063 616e 2061 6363 6573 7320 616c  ou can access al
-00001780: 6c20 7468 6569 7220 6869 7374 6f72 6963  l their historic
-00001790: 616c 202a 2a66 696c 696e 6773 2a2a 2c0a  al **filings**,.
-000017a0: 616e 6420 6120 6461 7461 7365 7420 6f66  and a dataset of
-000017b0: 2074 6865 2063 6f6d 7061 6e79 202a 2a66   the company **f
-000017c0: 6163 7473 2a2a 2e0a 5468 6520 5345 4327  acts**..The SEC'
-000017d0: 7320 636f 6d70 616e 7920 4150 4920 616c  s company API al
-000017e0: 736f 2073 7570 706c 6965 7320 6120 6c6f  so supplies a lo
-000017f0: 7420 6d6f 7265 2064 6574 6169 6c73 2061  t more details a
-00001800: 626f 7574 2061 2063 6f6d 7061 6e79 2069  bout a company i
-00001810: 6e63 6c75 6469 6e67 2069 6e64 7573 7472  ncluding industr
-00001820: 792c 2074 6865 2053 4543 2066 696c 6572  y, the SEC filer
-00001830: 2074 7970 652c 0a74 6865 206d 6169 6c69   type,.the maili
-00001840: 6e67 2061 6e64 2062 7573 696e 6573 7320  ng and business 
-00001850: 6164 6472 6573 7320 616e 6420 6d75 6368  address and much
-00001860: 206d 6f72 652e 0a0a 2323 2320 4669 6e64   more...### Find
-00001870: 2061 2063 6f6d 7061 6e79 2075 7369 6e67   a company using
-00001880: 2074 6865 2063 696b 0a54 6865 202a 2a63   the cik.The **c
-00001890: 696b 2a2a 2069 7320 7468 6520 6964 2074  ik** is the id t
-000018a0: 6861 7420 756e 6971 7565 6c79 2069 6465  hat uniquely ide
-000018b0: 6e74 6966 6965 7320 6120 636f 6d70 616e  ntifies a compan
-000018c0: 7920 6174 2074 6865 2053 4543 2e0a 4974  y at the SEC..It
-000018d0: 2069 7320 6120 6e75 6d62 6572 2c20 6275   is a number, bu
-000018e0: 7420 6973 2073 6f6d 6574 696d 6573 2073  t is sometimes s
-000018f0: 686f 776e 2069 6e20 5345 4320 4564 6761  hown in SEC Edga
-00001900: 7220 7265 736f 7572 6365 7320 6173 2061  r resources as a
-00001910: 2073 7472 696e 6720 7061 6464 6564 2077   string padded w
-00001920: 6974 6820 6c65 6164 696e 6720 7a65 726f  ith leading zero
-00001930: 2773 2e0a 466f 7220 7468 6520 6564 6761  's..For the edga
-00001940: 7220 636c 6965 6e74 2041 5049 2c20 6a75  r client API, ju
-00001950: 7374 2075 7365 2074 6865 206e 756d 6265  st use the numbe
-00001960: 7273 2061 6e64 206f 6d69 7420 7468 6520  rs and omit the 
-00001970: 6c65 6164 696e 6720 7a65 726f 6573 2e0a  leading zeroes..
-00001980: 0a60 6060 7079 7468 6f6e 0a63 6f6d 7061  .```python.compa
-00001990: 6e79 203d 2043 6f6d 7061 6e79 2831 3332  ny = Company(132
-000019a0: 3434 3234 290a 6060 600a 215b 6578 7065  4424).```.![expe
-000019b0: 5d28 6874 7470 733a 2f2f 7261 772e 6769  ](https://raw.gi
-000019c0: 7468 7562 7573 6572 636f 6e74 656e 742e  thubusercontent.
-000019d0: 636f 6d2f 6467 756e 6e69 6e67 2f65 6467  com/dgunning/edg
-000019e0: 6172 746f 6f6c 732f 6d61 696e 2f65 7870  artools/main/exp
-000019f0: 652e 706e 6729 0a0a 0a0a 2323 2320 4669  e.png)....### Fi
-00001a00: 6e64 2061 2063 6f6d 7061 6e79 2075 7369  nd a company usi
-00001a10: 6e67 2074 6963 6b65 720a 0a59 6f75 2063  ng ticker..You c
-00001a20: 616e 2067 6574 2061 2063 6f6d 7061 6e79  an get a company
-00001a30: 2075 7369 6e67 2061 2074 6963 6b65 7220   using a ticker 
-00001a40: 652e 672e 202a 2a53 4e4f 572a 2a2e 2054  e.g. **SNOW**. T
-00001a50: 6869 7320 7769 6c6c 2064 6f20 6120 6c6f  his will do a lo
-00001a60: 6f6b 7570 2066 6f72 2074 6865 2063 6f6d  okup for the com
-00001a70: 7061 6e79 2063 696b 2075 7369 6e67 2074  pany cik using t
-00001a80: 6865 2074 6963 6b65 722c 2074 6865 6e20  he ticker, then 
-00001a90: 6c6f 6164 2074 6865 2063 6f6d 7061 6e79  load the company
-00001aa0: 2075 7369 6e67 2074 6865 2063 696b 2e0a   using the cik..
-00001ab0: 5468 6973 206d 616b 6573 2069 7420 7477  This makes it tw
-00001ac0: 6f20 6361 6c6c 7320 7665 7273 7573 206f  o calls versus o
-00001ad0: 6e65 2066 6f72 2074 6865 2063 696b 2063  ne for the cik c
-00001ae0: 6f6d 7061 6e79 206c 6f6f 6b75 702c 2062  ompany lookup, b
-00001af0: 7574 2069 7320 736f 6d65 7469 6d65 7320  ut is sometimes 
-00001b00: 6d6f 7265 2063 6f6e 7665 6e69 656e 7420  more convenient 
-00001b10: 7369 6e63 6520 7469 636b 6572 7320 6172  since tickers ar
-00001b20: 6520 6561 7369 6572 2074 6f20 7265 6d65  e easier to reme
-00001b30: 6d62 6572 2074 6861 7420 6369 6b73 2e0a  mber that ciks..
-00001b40: 0a4e 6f74 6520 7468 6174 2073 6f6d 6520  .Note that some 
-00001b50: 636f 6d70 616e 6965 7320 6861 7665 206d  companies have m
-00001b60: 756c 7469 706c 6520 7469 636b 6572 732c  ultiple tickers,
-00001b70: 2073 6f20 796f 7520 7465 6368 6e69 6361   so you technica
-00001b80: 6c6c 7920 6361 6e6e 6f74 2067 6574 2053  lly cannot get S
-00001b90: 4543 2066 696c 696e 6773 2066 6f72 2061  EC filings for a
-00001ba0: 2074 6963 6b65 722e 0a59 6f75 2069 6e73   ticker..You ins
-00001bb0: 7465 6164 2067 6574 2074 6865 2053 4543  tead get the SEC
-00001bc0: 2066 696c 696e 6773 2066 6f72 2074 6865   filings for the
-00001bd0: 2063 6f6d 7061 6e79 2074 6f20 7768 6963   company to whic
-00001be0: 6820 7468 6520 7469 636b 6572 2062 656c  h the ticker bel
-00001bf0: 6f6e 6773 2e0a 0a54 6865 2074 6963 6b65  ongs...The ticke
-00001c00: 7220 6973 2063 6173 652d 696e 7365 6e73  r is case-insens
-00001c10: 6974 6976 6520 736f 2079 6f75 2063 616e  itive so you can
-00001c20: 2075 7365 2060 436f 6d70 616e 7928 2273   use `Company("s
-00001c30: 6e6f 7722 2960 0a6f 7220 6043 6f6d 7061  now")`.or `Compa
-00001c40: 6e79 2822 534e 4f57 2229 600a 6060 6070  ny("SNOW")`.```p
-00001c50: 7974 686f 6e0a 736e 6f77 203d 2043 6f6d  ython.snow = Com
-00001c60: 7061 6e79 2822 736e 6f77 2229 0a60 6060  pany("snow").```
-00001c70: 0a0a 215b 736e 6f77 2069 6e73 7065 6374  ..![snow inspect
-00001c80: 5d28 6874 7470 733a 2f2f 7261 772e 6769  ](https://raw.gi
-00001c90: 7468 7562 7573 6572 636f 6e74 656e 742e  thubusercontent.
-00001ca0: 636f 6d2f 6467 756e 6e69 6e67 2f65 6467  com/dgunning/edg
-00001cb0: 6172 746f 6f6c 732f 6d61 696e 2f73 6e6f  artools/main/sno
-00001cc0: 772d 696e 7370 6563 742e 706e 6729 0a23  w-inspect.png).#
-00001cd0: 2323 200a 0a0a 6060 6070 7974 686f 6e0a  ## ...```python.
-00001ce0: 436f 6d70 616e 7928 3138 3332 3935 3029  Company(1832950)
-00001cf0: 0a60 6060 0a0a 2323 2320 4765 7420 6669  .```..### Get fi
-00001d00: 6c69 6e67 7320 666f 7220 6120 636f 6d70  lings for a comp
-00001d10: 616e 790a 546f 2067 6574 2074 6865 2063  any.To get the c
-00001d20: 6f6d 7061 6e79 2773 2066 696c 696e 6773  ompany's filings
-00001d30: 2075 7365 2060 6765 745f 6669 6c69 6e67   use `get_filing
-00001d40: 7328 2960 2e20 5468 6973 2067 6574 7320  s()`. This gets 
-00001d50: 616c 6c20 7468 6520 636f 6d70 616e 7927  all the company'
-00001d60: 7320 6669 6c69 6e67 7320 7468 6174 2061  s filings that a
-00001d70: 7265 2061 7661 696c 6162 6c65 2066 726f  re available fro
-00001d80: 6d20 7468 6520 4564 6761 7220 7375 626d  m the Edgar subm
-00001d90: 6973 7369 6f6e 7320 656e 6470 6f69 6e74  issions endpoint
-00001da0: 2e0a 0a60 6060 7079 7468 6f6e 0a63 6f6d  ...```python.com
-00001db0: 7061 6e79 2e67 6574 5f66 696c 696e 6773  pany.get_filings
-00001dc0: 2829 0a60 6060 0a23 2323 2046 696c 7465  ().```.### Filte
-00001dd0: 7269 6e67 2066 696c 696e 6773 0a59 6f75  ring filings.You
-00001de0: 2063 616e 2066 696c 7465 7220 7468 6520   can filter the 
-00001df0: 636f 6d70 616e 7920 6669 6c69 6e67 7320  company filings 
-00001e00: 7573 696e 6720 6120 6e75 6d62 6572 206f  using a number o
-00001e10: 6620 6469 6666 6572 656e 7420 7061 7261  f different para
-00001e20: 6d65 7465 7273 2e0a 0a60 6060 7079 7468  meters...```pyth
-00001e30: 6f6e 0a63 6c61 7373 2043 6f6d 7061 6e79  on.class Company
-00001e40: 4669 6c69 6e67 733a 0a20 2020 200a 2020  Filings:.    .  
-00001e50: 2020 2e2e 2e0a 2020 2020 0a20 2020 2064    ....    .    d
-00001e60: 6566 2067 6574 5f66 696c 696e 6773 2873  ef get_filings(s
-00001e70: 656c 662c 0a20 2020 2020 2020 2020 2020  elf,.           
-00001e80: 2020 2020 2020 2020 202a 2c0a 2020 2020           *,.    
-00001e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001ea0: 666f 726d 3a20 7374 7220 7c20 4c69 7374  form: str | List
-00001eb0: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
-00001ec0: 2020 2020 2020 2020 2020 2020 2061 6363               acc
-00001ed0: 6573 7369 6f6e 5f6e 756d 6265 723a 2073  ession_number: s
-00001ee0: 7472 207c 204c 6973 7420 3d20 4e6f 6e65  tr | List = None
-00001ef0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00001f00: 2020 2020 2020 6669 6c65 5f6e 756d 6265        file_numbe
-00001f10: 723a 2073 7472 207c 204c 6973 7420 3d20  r: str | List = 
-00001f20: 4e6f 6e65 2c0a 2020 2020 2020 2020 2020  None,.          
-00001f30: 2020 2020 2020 2020 2020 6973 5f78 6272            is_xbr
-00001f40: 6c3a 2062 6f6f 6c20 3d20 4e6f 6e65 2c0a  l: bool = None,.
-00001f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001f60: 2020 2020 6973 5f69 6e6c 696e 655f 7862      is_inline_xb
-00001f70: 726c 3a20 626f 6f6c 203d 204e 6f6e 650a  rl: bool = None.
-00001f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001f90: 2020 2020 293a 0a20 2020 2020 2020 2022      ):.        "
-00001fa0: 2222 0a20 2020 2020 2020 2047 6574 2074  "".        Get t
-00001fb0: 6865 2063 6f6d 7061 6e79 2773 2066 696c  he company's fil
-00001fc0: 696e 6773 2061 6e64 206f 7074 696f 6e61  ings and optiona
-00001fd0: 6c6c 7920 6669 6c74 6572 2062 7920 6d75  lly filter by mu
-00001fe0: 6c74 6970 6c65 2063 7269 7465 7269 610a  ltiple criteria.
-00001ff0: 2020 2020 2020 2020 3a70 6172 616d 2066          :param f
-00002000: 6f72 6d3a 2054 6865 2066 6f72 6d20 6173  orm: The form as
-00002010: 2061 2073 7472 696e 6720 652e 672e 2027   a string e.g. '
-00002020: 3130 2d4b 2720 6f72 204c 6973 7420 6f66  10-K' or List of
-00002030: 2073 7472 696e 6773 205b 2731 302d 5127   strings ['10-Q'
-00002040: 2c20 2731 302d 4b27 5d0a 2020 2020 2020  , '10-K'].      
-00002050: 2020 3a70 6172 616d 2061 6363 6573 7369    :param accessi
-00002060: 6f6e 5f6e 756d 6265 723a 2054 6865 2061  on_number: The a
-00002070: 6363 6573 7369 6f6e 206e 756d 6265 7220  ccession number 
-00002080: 7468 6174 2075 6e69 7175 656c 7920 6964  that uniquely id
-00002090: 656e 7469 6669 6573 2061 6e20 5345 4320  entifies an SEC 
-000020a0: 6669 6c69 6e67 2065 2e67 2e20 3030 3031  filing e.g. 0001
-000020b0: 3634 3031 3437 2d32 322d 3030 3031 3030  640147-22-000100
-000020c0: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
-000020d0: 6669 6c65 5f6e 756d 6265 723a 2054 6865  file_number: The
-000020e0: 2066 696c 6520 6e75 6d62 6572 2065 2e67   file number e.g
-000020f0: 2e20 3030 312d 3339 3530 340a 2020 2020  . 001-39504.    
-00002100: 2020 2020 3a70 6172 616d 2069 735f 7862      :param is_xb
-00002110: 726c 3a20 5768 6574 6865 7220 7468 6520  rl: Whether the 
-00002120: 6669 6c69 6e67 2069 7320 7862 726c 0a20  filing is xbrl. 
-00002130: 2020 2020 2020 203a 7061 7261 6d20 6973         :param is
-00002140: 5f69 6e6c 696e 655f 7862 726c 3a20 5768  _inline_xbrl: Wh
-00002150: 6574 6865 7220 7468 6520 6669 6c69 6e67  ether the filing
-00002160: 2069 7320 696e 6c69 6e65 5f78 6272 6c0a   is inline_xbrl.
-00002170: 2020 2020 2020 2020 3a72 6574 7572 6e3a          :return:
-00002180: 2054 6865 2043 6f6d 7061 6e79 4669 6c69   The CompanyFili
-00002190: 6e67 2069 6e73 7461 6e63 6520 7769 7468  ng instance with
-000021a0: 2074 6865 2066 696c 696e 6773 2074 6861   the filings tha
-000021b0: 7420 6d61 7463 6820 7468 6520 6669 6c74  t match the filt
-000021c0: 6572 730a 2020 2020 2020 2020 2222 220a  ers.        """.
-000021d0: 6060 600a 0a0a 2323 2323 2054 6865 2043  ```...#### The C
-000021e0: 6f6d 7061 6e79 4669 6c69 6e67 7320 636c  ompanyFilings cl
-000021f0: 6173 730a 5468 6520 7265 7375 6c74 206f  ass.The result o
-00002200: 6620 6067 6574 5f66 696c 696e 6773 2829  f `get_filings()
-00002210: 6020 6973 2061 2060 436f 6d70 616e 7946  ` is a `CompanyF
-00002220: 696c 696e 6773 6020 636c 6173 732e 2054  ilings` class. T
-00002230: 6869 7320 636c 6173 7320 636f 6e74 6169  his class contai
-00002240: 6e73 2061 2070 7961 7272 6f77 2074 6162  ns a pyarrow tab
-00002250: 6c65 2077 6974 6820 7468 6520 6669 6c69  le with the fili
-00002260: 6e67 730a 616e 6420 7072 6f76 6964 6573  ngs.and provides
-00002270: 2063 6f6e 7665 6e69 656e 7420 6675 6e63   convenient func
-00002280: 7469 6f6e 7320 666f 7220 776f 726b 696e  tions for workin
-00002290: 6720 7769 7468 2066 696c 696e 6773 2e0a  g with filings..
-000022a0: 596f 7520 6361 6e20 6163 6365 7373 2074  You can access t
-000022b0: 6865 2075 6e64 6572 6c79 696e 6720 7079  he underlying py
-000022c0: 6172 726f 7720 6054 6162 6c65 6020 7573  arrow `Table` us
-000022d0: 696e 6720 7468 6520 602e 6461 7461 6020  ing the `.data` 
-000022e0: 7072 6f70 6572 7479 0a0a 6060 6070 7974  property..```pyt
-000022f0: 686f 6e0a 6669 6c69 6e67 7320 3d20 636f  hon.filings = co
-00002300: 6d70 616e 792e 6765 745f 6669 6c69 6e67  mpany.get_filing
-00002310: 7328 290a 0a23 2047 6574 2074 6865 2075  s()..# Get the u
-00002320: 6e64 6572 6c79 696e 6720 5461 626c 650a  nderlying Table.
-00002330: 6461 7461 3a20 7061 2e54 6162 6c65 203d  data: pa.Table =
-00002340: 2066 696c 696e 6773 2e64 6174 610a 6060   filings.data.``
-00002350: 600a 0a23 2323 2320 4765 7420 6120 6669  `..#### Get a fi
-00002360: 6c69 6e67 2062 7920 696e 6465 780a 546f  ling by index.To
-00002370: 2061 6363 6573 7320 6120 6669 6c69 6e67   access a filing
-00002380: 2069 6e20 7468 6520 436f 6d70 616e 7946   in the CompanyF
-00002390: 696c 696e 6773 2075 7365 2074 6865 2062  ilings use the b
-000023a0: 7261 636b 6574 2060 5b5d 6020 6e6f 7461  racket `[]` nota
-000023b0: 7469 6f6e 2065 2e67 2e20 6066 696c 696e  tion e.g. `filin
-000023c0: 6773 5b32 5d60 0a60 6060 7079 7468 6f6e  gs[2]`.```python
-000023d0: 0a66 696c 696e 6773 5b32 5d0a 6060 600a  .filings[2].```.
-000023e0: 0a23 2323 2320 4765 7420 7468 6520 6c61  .#### Get the la
-000023f0: 7465 7374 2066 696c 696e 670a 0a54 6865  test filing..The
-00002400: 2060 436f 6d70 616e 7946 696c 696e 6773   `CompanyFilings
-00002410: 6020 636c 6173 7320 6861 7320 6120 606c  ` class has a `l
-00002420: 6174 6573 7460 2066 756e 6374 696f 6e20  atest` function 
-00002430: 7468 6174 2077 696c 6c20 7265 7475 726e  that will return
-00002440: 2074 6865 206c 6174 6573 7420 6046 696c   the latest `Fil
-00002450: 696e 6760 2e20 0a53 6f2c 2074 6f20 6765  ing`. .So, to ge
-00002460: 7420 7468 6520 6c61 7465 7374 202a 2a31  t the latest **1
-00002470: 302d 512a 2a20 6669 6c69 6e67 2c20 796f  0-Q** filing, yo
-00002480: 7520 646f 2074 6865 2066 6f6c 6c6f 7769  u do the followi
-00002490: 6e67 0a60 6060 7079 7468 6f6e 0a23 204c  ng.```python.# L
-000024a0: 6174 6573 7420 6669 6c69 6e67 206d 616b  atest filing mak
-000024b0: 6573 2073 656e 7365 2069 6620 796f 7520  es sense if you 
-000024c0: 6669 6c74 6572 2062 7920 666f 726d 2020  filter by form  
-000024d0: 7479 7065 2065 2e67 2e20 3130 2d51 0a73  type e.g. 10-Q.s
-000024e0: 6e6f 775f 3130 5173 203d 2073 6e6f 772e  now_10Qs = snow.
-000024f0: 6765 745f 6669 6c69 6e67 7328 666f 726d  get_filings(form
-00002500: 3d27 3130 2d51 2729 0a6c 6174 6573 745f  ='10-Q').latest_
-00002510: 3130 5120 3d20 736e 6f77 5f31 3051 732e  10Q = snow_10Qs.
-00002520: 6c61 7465 7374 2829 0a0a 2320 4f72 2063  latest()..# Or c
-00002530: 6861 696e 2074 6865 2066 756e 6374 696f  hain the functio
-00002540: 6e20 6361 6c6c 730a 736e 6f77 2e67 6574  n calls.snow.get
-00002550: 5f66 696c 696e 6773 2866 6f72 6d3d 2731  _filings(form='1
-00002560: 302d 5127 292e 6c61 7465 7374 2829 0a60  0-Q').latest().`
-00002570: 6060 0a0a 0a23 2323 2047 6574 2063 6f6d  ``...### Get com
-00002580: 7061 6e79 2066 6163 7473 0a0a 4661 6374  pany facts..Fact
-00002590: 7320 6172 6520 616e 2069 6e74 6572 6573  s are an interes
-000025a0: 7469 6e67 2061 6e64 2069 6d70 6f72 7461  ting and importa
-000025b0: 6e74 2064 6174 6173 6574 2061 626f 7574  nt dataset about
-000025c0: 2061 2063 6f6d 7061 6e79 2061 6363 756d   a company accum
-000025d0: 6c61 7465 6420 6672 6f6d 2064 6174 6120  lated from data 
-000025e0: 7468 6520 636f 6d70 616e 7920 7072 6f76  the company prov
-000025f0: 6964 6573 2074 6f20 7468 6520 5345 432e  ides to the SEC.
-00002600: 0a43 6f6d 7061 6e79 2066 6163 7473 2061  .Company facts a
-00002610: 7265 2061 7661 696c 6162 6c65 2066 6f72  re available for
-00002620: 2061 2063 6f6d 7061 6e79 206f 6e20 7468   a company on th
-00002630: 6520 436f 6d70 616e 7920 4661 6374 7360  e Company Facts`
-00002640: 6622 6874 7470 733a 2f2f 6461 7461 2e73  f"https://data.s
-00002650: 6563 2e67 6f76 2f61 7069 2f78 6272 6c2f  ec.gov/api/xbrl/
-00002660: 636f 6d70 616e 7966 6163 7473 2f43 494b  companyfacts/CIK
-00002670: 7b63 696b 3a30 3130 7d2e 6a73 6f6e 2260  {cik:010}.json"`
-00002680: 0a49 7420 6973 2061 204a 534f 4e20 656e  .It is a JSON en
-00002690: 6470 6f69 6e74 2061 6e64 2060 6564 6761  dpoint and `edga
-000026a0: 7274 6f6f 6c73 6020 7061 7273 6573 2074  rtools` parses t
-000026b0: 6865 204a 534f 4e20 696e 746f 2061 2073  he JSON into a s
-000026c0: 7472 7563 7475 7265 6420 6461 7461 7365  tructured datase
-000026d0: 7420 2d20 6120 6070 7961 7272 6f77 2e54  t - a `pyarrow.T
-000026e0: 6162 6c65 602e 0a0a 2323 2323 2047 6574  able`...#### Get
-000026f0: 7469 6e67 2066 6163 7473 2066 6f72 2061  ting facts for a
-00002700: 2063 6f6d 7061 6e79 0a54 6f20 6765 7420   company.To get 
-00002710: 636f 6d70 616e 7920 6661 6374 732c 2066  company facts, f
-00002720: 6972 7374 2067 6574 2074 6865 2063 6f6d  irst get the com
-00002730: 7061 6e79 2c20 7468 656e 2063 616c 6c20  pany, then call 
-00002740: 6063 6f6d 7061 6e79 2e67 6574 5f66 6163  `company.get_fac
-00002750: 7473 2829 600a 6060 6070 7974 686f 6e0a  ts()`.```python.
-00002760: 636f 6d70 616e 7920 3d20 436f 6d70 616e  company = Compan
-00002770: 7928 2253 4e4f 5722 290a 636f 6d70 616e  y("SNOW").compan
-00002780: 795f 6661 6374 7320 3d20 636f 6d70 616e  y_facts = compan
-00002790: 792e 6765 745f 6661 6374 7328 290a 6060  y.get_facts().``
-000027a0: 600a 5468 6520 7265 7375 6c74 2069 7320  `.The result is 
-000027b0: 6120 6043 6f6d 7061 6e79 4661 6374 7360  a `CompanyFacts`
-000027c0: 206f 626a 6563 7420 7768 6963 6820 7772   object which wr
-000027d0: 6170 7320 7468 6520 756e 6465 726c 7969  aps the underlyi
-000027e0: 6e67 2066 6163 7473 2061 6e64 2070 726f  ng facts and pro
-000027f0: 7669 6465 7320 636f 6e76 656e 6965 6e74  vides convenient
-00002800: 2077 6179 7320 6f66 2077 6f72 6b69 6e67   ways of working
-00002810: 0a77 6974 6820 7468 6520 6661 6374 7320  .with the facts 
-00002820: 6461 7461 2e20 546f 2067 6574 2061 6363  data. To get acc
-00002830: 6573 7320 746f 2074 6865 2075 6e64 6572  ess to the under
-00002840: 796c 696e 6720 6461 7461 2075 7365 2074  yling data use t
-00002850: 6865 2060 6661 6374 7360 2070 726f 7065  he `facts` prope
-00002860: 7274 792e 0a0a 596f 7520 6361 6e20 6765  rty...You can ge
-00002870: 7420 7468 6520 6661 6374 7320 6173 2061  t the facts as a
-00002880: 2070 616e 6461 7320 6461 7461 6672 616d   pandas datafram
-00002890: 6520 6279 2063 616c 6c69 6e67 2060 746f  e by calling `to
-000028a0: 5f70 616e 6461 7360 0a0a 6060 6070 7974  _pandas`..```pyt
-000028b0: 686f 6e0a 6466 203d 2063 6f6d 7061 6e79  hon.df = company
-000028c0: 5f66 6163 7473 2e74 6f5f 7061 6e64 6173  _facts.to_pandas
-000028d0: 2829 0a60 6060 0a0a 4661 6374 7320 6469  ().```..Facts di
-000028e0: 6666 6572 2061 6d6f 6e67 2063 6f6d 7061  ffer among compa
-000028f0: 6e69 6573 2e20 546f 2073 6565 2077 6861  nies. To see wha
-00002900: 7420 6661 6374 7320 6172 6520 6176 6169  t facts are avai
-00002910: 6c61 626c 6520 796f 7520 6361 6e20 7573  lable you can us
-00002920: 6520 7468 6520 6066 6163 7473 5f6d 6574  e the `facts_met
-00002930: 6160 2070 726f 7065 7274 792e 0a0a 2323  a` property...##
-00002940: 2323 2047 6574 7469 6e67 2074 6865 2066  ## Getting the f
-00002950: 6163 7473 2061 7320 6120 4475 636b 4442  acts as a DuckDB
-00002960: 2074 6162 6c65 0a59 7075 2063 616e 2063   table.Ypu can c
-00002970: 6f6e 7665 7274 2074 6865 2066 6163 7473  onvert the facts
-00002980: 2074 6f20 6120 4475 636b 4442 2064 6174   to a DuckDB dat
-00002990: 6162 6173 6520 7768 6963 6820 616c 6c6f  abase which allo
-000029a0: 7773 2079 6f75 2074 6f20 7175 6572 7920  ws you to query 
-000029b0: 7468 6520 6661 6374 7320 7573 696e 6720  the facts using 
-000029c0: 5351 4c2e 0a0a 6060 6070 7974 686f 6e0a  SQL...```python.
-000029d0: 2020 2020 636f 6d70 616e 795f 6661 6374      company_fact
-000029e0: 733a 2043 6f6d 7061 6e79 4661 6374 7320  s: CompanyFacts 
-000029f0: 3d20 6765 745f 636f 6d70 616e 795f 6661  = get_company_fa
-00002a00: 6374 7328 3133 3138 3630 3529 0a20 2020  cts(1318605).   
-00002a10: 2064 6220 3d20 636f 6d70 616e 795f 6661   db = company_fa
-00002a20: 6374 732e 746f 5f64 7563 6b64 6228 290a  cts.to_duckdb().
-00002a30: 2020 2020 6466 203d 2064 622e 6578 6563      df = db.exec
-00002a40: 7574 6528 2222 220a 2020 2020 7365 6c65  ute(""".    sele
-00002a50: 6374 202a 2066 726f 6d20 6661 6374 730a  ct * from facts.
-00002a60: 2020 2020 2222 2229 2e64 6628 290a 6060      """).df().``
-00002a70: 600a 0a0a 0a23 2320 576f 726b 696e 6720  `....## Working 
-00002a80: 7769 7468 2061 2046 696c 696e 670a 0a4f  with a Filing..O
-00002a90: 6e63 6520 796f 7520 6861 7665 2061 2066  nce you have a f
-00002aa0: 696c 696e 6720 796f 7520 6361 6e20 646f  iling you can do
-00002ab0: 206d 616e 7920 7468 696e 6773 2077 6974   many things wit
-00002ac0: 6820 6974 2069 6e63 6c75 6469 6e67 2067  h it including g
-00002ad0: 6574 7469 6e67 2074 6865 2068 746d 6c20  etting the html 
-00002ae0: 7465 7874 206f 6620 7468 6520 6669 6c69  text of the fili
-00002af0: 6e67 2c20 6765 7420 7862 726c 206f 7220  ng, get xbrl or 
-00002b00: 786d 6c2c 206f 7220 6c69 7374 2061 6c6c  xml, or list all
-00002b10: 2074 6865 2066 696c 6573 2069 6e20 7468   the files in th
-00002b20: 6520 6669 6c69 6e67 2e0a 0a23 2323 2047  e filing...### G
-00002b30: 6574 7469 6e67 2074 6865 2068 746d 6c20  etting the html 
-00002b40: 7465 7874 206f 6620 6120 6669 6c69 6e67  text of a filing
-00002b50: 0a0a 6060 6070 7974 686f 6e0a 6874 6d6c  ..```python.html
-00002b60: 203d 2066 696c 696e 672e 6874 6d6c 2829   = filing.html()
-00002b70: 0a60 6060 0a0a 0a54 6f20 6765 7420 7468  .```...To get th
-00002b80: 6520 6874 6d6c 2074 6578 7420 6f66 2074  e html text of t
-00002b90: 6865 2066 696c 696e 6720 6361 6c6c 2060  he filing call `
-00002ba0: 6669 6c69 6e67 2e68 746d 6c28 2960 0a0a  filing.html()`..
-00002bb0: 2323 2320 4765 7420 7468 6520 486f 6d65  ### Get the Home
-00002bc0: 7061 6765 2055 726c 0a0a 6066 696c 696e  page Url..`filin
-00002bd0: 672e 686f 6d65 7061 6765 5f75 726c 6020  g.homepage_url` 
-00002be0: 7265 7475 726e 7320 7468 6520 686f 6d65  returns the home
-00002bf0: 7061 6765 2075 726c 206f 6620 7468 6520  page url of the 
-00002c00: 6669 6c69 6e67 2e20 5468 6973 2069 7320  filing. This is 
-00002c10: 7468 6520 6d61 696e 2069 6e64 6578 2070  the main index p
-00002c20: 6167 6520 7768 6963 6820 6c69 7374 730a  age which lists.
-00002c30: 616c 6c20 7468 6520 6669 6c65 7320 6174  all the files at
-00002c40: 7461 6368 6564 2069 6e20 7468 6520 6669  tached in the fi
-00002c50: 6c69 6e67 0a0a 2323 2320 4765 7420 7468  ling..### Get th
-00002c60: 6520 6669 6c69 6e67 2068 6f6d 6570 6167  e filing homepag
-00002c70: 650a 0a54 6f20 6765 7420 6163 6365 7373  e..To get access
-00002c80: 2074 6f20 616c 6c20 7468 6520 646f 6375   to all the docu
-00002c90: 6d65 6e74 7320 6f6e 2074 6865 2066 696c  ments on the fil
-00002ca0: 696e 6720 796f 7520 776f 756c 6420 6361  ing you would ca
-00002cb0: 6c6c 2060 6669 6c69 6e67 2e67 6574 5f68  ll `filing.get_h
-00002cc0: 6f6d 6570 6167 6528 2960 2e0a 5468 6973  omepage()`..This
-00002cd0: 2067 6976 6573 2079 6f75 2061 6363 6573   gives you acces
-00002ce0: 7320 746f 2074 6865 2060 4669 6c69 6e67  s to the `Filing
-00002cf0: 486f 6d65 7061 6765 6020 636c 6173 7320  Homepage` class 
-00002d00: 7468 6174 2079 6f75 2063 616e 2075 7365  that you can use
-00002d10: 2074 6f20 6c69 7374 2061 6c6c 2074 6865   to list all the
-00002d20: 2064 6f63 756d 656e 7473 0a61 6e64 2064   documents.and d
-00002d30: 6174 6166 696c 6573 206f 6e20 7468 6520  atafiles on the 
-00002d40: 6669 6c69 6e67 2e0a 0a0a 2323 2320 576f  filing....### Wo
-00002d50: 726b 696e 6720 7769 7468 2058 4252 4c20  rking with XBRL 
-00002d60: 6669 6c69 6e67 730a 0a53 6f6d 6520 6669  filings..Some fi
-00002d70: 6c69 6e67 7320 6172 6520 696e 202a 2a58  lings are in **X
-00002d80: 4252 4c20 2865 5874 656e 7369 626c 6520  BRL (eXtensible 
-00002d90: 4275 7369 6e65 7373 204d 6172 6b75 7020  Business Markup 
-00002da0: 4c61 6e67 7561 6765 292a 2a20 666f 726d  Language)** form
-00002db0: 6174 2e20 0a54 6865 7365 2061 7265 206d  at. .These are m
-00002dc0: 6169 6e6c 7920 7468 6520 6e65 7765 7220  ainly the newer 
-00002dd0: 6669 6c69 6e67 732c 2061 7320 7468 6520  filings, as the 
-00002de0: 5345 4320 6861 7320 7374 6172 7465 6420  SEC has started 
-00002df0: 7265 7175 6972 696e 6720 7468 6973 2066  requiring this f
-00002e00: 6f72 206e 6577 6572 2066 696c 696e 6773  or newer filings
-00002e10: 2e0a 0a49 6620 6120 6669 6c69 6e67 2069  ...If a filing i
-00002e20: 7320 696e 2058 4252 4c20 666f 726d 6174  s in XBRL format
-00002e30: 2074 6865 6e20 6974 206f 7065 6e73 2075   then it opens u
-00002e40: 7020 6120 6c6f 7420 6d6f 7265 2077 6179  p a lot more way
-00002e50: 7320 746f 2067 6574 2073 7472 7563 7475  s to get structu
-00002e60: 7265 6420 6461 7461 2061 626f 7574 2074  red data about t
-00002e70: 6861 7420 7370 6563 6966 6963 2066 696c  hat specific fil
-00002e80: 696e 6720 616e 6420 616c 736f 200a 6162  ing and also .ab
-00002e90: 6f75 7420 7468 6520 636f 6d70 616e 7920  out the company 
-00002ea0: 7265 6665 7272 6564 2074 6f20 696e 2074  referred to in t
-00002eb0: 6861 7420 6669 6c69 6e67 2e0a 0a54 6865  hat filing...The
-00002ec0: 2060 4669 6c69 6e67 6020 636c 6173 7320   `Filing` class 
-00002ed0: 6861 7320 616e 2060 7862 726c 6020 6675  has an `xbrl` fu
-00002ee0: 6e63 7469 6f6e 2074 6861 7420 7769 6c6c  nction that will
-00002ef0: 2064 6f77 6e6c 6f61 642c 2070 6172 7365   download, parse
-00002f00: 2061 6e64 2073 7472 7563 7475 7265 2074   and structure t
-00002f10: 6865 2066 696c 696e 6727 7320 5842 524c  he filing's XBRL
-00002f20: 2064 6f63 756d 656e 7420 6966 206f 6e65   document if one
-00002f30: 2065 7869 7374 732e 0a49 6620 6974 2064   exists..If it d
-00002f40: 6f65 7320 6e6f 7420 6578 6973 742c 2074  oes not exist, t
-00002f50: 6865 6e20 6066 696c 696e 672e 7862 726c  hen `filing.xbrl
-00002f60: 2829 6020 7769 6c6c 2072 6574 7572 6e20  ()` will return 
-00002f70: 604e 6f6e 6560 2e0a 0a54 6865 2066 756e  `None`...The fun
-00002f80: 6374 696f 6e20 6066 696c 696e 672e 7862  ction `filing.xb
-00002f90: 726c 2829 6020 7265 7475 726e 7320 6120  rl()` returns a 
-00002fa0: 6046 696c 696e 6758 6272 6c60 2069 6e73  `FilingXbrl` ins
-00002fb0: 7461 6e63 652c 2077 6869 6368 2077 7261  tance, which wra
-00002fc0: 7073 2074 6865 2064 6174 612c 2061 6e64  ps the data, and
-00002fd0: 2070 726f 7669 6465 7320 636f 6e76 656e   provides conven
-00002fe0: 6965 6e74 0a77 6179 7320 6f66 2077 6f72  ient.ways of wor
-00002ff0: 6b69 6e67 2077 6974 6820 7468 6520 7862  king with the xb
-00003000: 726c 2064 6174 612e 0a0a 0a60 6060 7079  rl data....```py
-00003010: 7468 6f6e 0a66 696c 696e 675f 7862 726c  thon.filing_xbrl
-00003020: 203d 2066 696c 696e 672e 7862 726c 2829   = filing.xbrl()
-00003030: 0a60 6060 0a0a 2323 2055 7369 6e67 2074  .```..## Using t
-00003040: 6865 2046 696c 696e 6773 2041 5049 0a0a  he Filings API..
-00003050: 5468 6520 2a2a 4669 6c69 6e67 7320 4150  The **Filings AP
-00003060: 492a 2a20 616c 6c6f 7773 2079 6f75 2074  I** allows you t
-00003070: 6f20 6765 7420 7468 6520 4564 6761 7220  o get the Edgar 
-00003080: 6669 6c69 6e67 2069 6e64 6578 6573 2070  filing indexes p
-00003090: 7562 6c69 7368 6564 2062 7920 7468 6520  ublished by the 
-000030a0: 5345 432e 0a59 6f75 2077 6f75 6c64 2075  SEC..You would u
-000030b0: 7365 2069 7420 746f 2067 6574 2061 2062  se it to get a b
-000030c0: 756c 6b20 6461 7461 7365 7420 6f66 2053  ulk dataset of S
-000030d0: 4543 2066 696c 696e 6773 2066 6f72 2061  EC filings for a
-000030e0: 2067 6976 656e 2074 696d 6520 7065 7269   given time peri
-000030f0: 6f64 2e20 5769 7468 2074 6869 7320 6461  od. With this da
-00003100: 7461 7365 742c 2079 6f75 2063 6f75 6c64  taset, you could
-00003110: 2066 696c 7465 7220 6279 2066 6f72 6d20   filter by form 
-00003120: 7479 7065 2c20 6279 2064 6174 6520 6f72  type, by date or
-00003130: 2062 7920 636f 6d70 616e 792c 200a 7468   by company, .th
-00003140: 6f75 6768 2069 6620 796f 7520 696e 7465  ough if you inte
-00003150: 6e64 2074 6f20 6669 6c74 6572 2062 7920  nd to filter by 
-00003160: 6120 7369 6e67 6520 636f 6d70 616e 792c  a singe company,
-00003170: 2079 6f75 2073 686f 756c 6420 7573 6520   you should use 
-00003180: 7468 6520 436f 6d70 616e 7920 4150 492e  the Company API.
-00003190: 0a0a 2323 2320 5468 6520 6765 745f 6669  ..### The get_fi
-000031a0: 6c69 6e67 7320 6675 6e63 7469 6f6e 0a54  lings function.T
-000031b0: 6865 206d 6169 6e20 7761 7920 746f 2075  he main way to u
-000031c0: 7365 2074 6865 2046 696c 696e 6773 2041  se the Filings A
-000031d0: 5049 2069 7320 6279 2060 6765 745f 6669  PI is by `get_fi
-000031e0: 6c69 6e67 7360 0a0a 6067 6574 5f66 696c  lings`..`get_fil
-000031f0: 696e 6773 6020 6163 6365 7074 7320 7468  ings` accepts th
-00003200: 6520 666f 6c6c 6f77 696e 6720 7061 7261  e following para
-00003210: 6d65 7465 7273 0a2d 202a 2a79 6561 722a  meters.- **year*
-00003220: 2a20 6120 7965 6172 2060 3230 3135 602c  * a year `2015`,
-00003230: 2061 204c 6973 7420 6f66 2079 6561 7273   a List of years
-00003240: 2060 5b32 3031 332c 2032 3031 355d 6020   `[2013, 2015]` 
-00003250: 6f72 2061 2060 7261 6e67 6528 3230 3133  or a `range(2013
-00003260: 2c20 3230 3136 2960 200a 2d20 2a2a 7175  , 2016)` .- **qu
-00003270: 6172 7465 722a 2a20 6120 7175 6172 7465  arter** a quarte
-00003280: 7220 6032 602c 2061 204c 6973 7420 6f66  r `2`, a List of
-00003290: 2071 7561 7274 6572 7320 605b 312c 322c   quarters `[1,2,
-000032a0: 335d 6020 6f72 2061 2060 7261 6e67 6528  3]` or a `range(
-000032b0: 312c 3329 6020 0a2d 202a 2a69 6e64 6578  1,3)` .- **index
-000032c0: 2a2a 2074 6869 7320 6973 2074 6865 2074  ** this is the t
-000032d0: 7970 6520 6f66 2069 6e64 6578 2e20 4279  ype of index. By
-000032e0: 2064 6566 6175 6c74 2069 7420 6973 2060   default it is `
-000032f0: 2266 6f72 6d22 602e 2049 6620 796f 7520  "form"`. If you 
-00003300: 7761 6e74 206f 6e6c 7920 5842 524c 2066  want only XBRL f
-00003310: 696c 696e 6773 2075 7365 2060 2278 6272  ilings use `"xbr
-00003320: 6c22 602e 200a 596f 7520 6361 6e20 616c  l"`. .You can al
-00003330: 736f 2075 7365 2060 2263 6f6d 7061 6e79  so use `"company
-00003340: 2260 2062 7574 2074 6869 7320 7769 6c6c  "` but this will
-00003350: 2067 6976 6520 796f 7520 7468 6520 7361   give you the sa
-00003360: 6d65 2064 6174 6173 6574 2061 7320 6022  me dataset as `"
-00003370: 666f 726d 2260 2c20 736f 7274 6564 2062  form"`, sorted b
-00003380: 7920 636f 6d70 616e 7920 696e 7374 6561  y company instea
-00003390: 6420 6f66 2062 7920 666f 726d 0a0a 2323  d of by form..##
-000033a0: 2323 2047 6574 2066 696c 696e 6773 2066  ## Get filings f
-000033b0: 6f72 2032 3032 310a 0a60 6060 7079 7468  or 2021..```pyth
-000033c0: 6f6e 0a66 696c 696e 6773 203d 2067 6574  on.filings = get
-000033d0: 5f66 696c 696e 6773 2832 3032 3129 0a60  _filings(2021).`
-000033e0: 6060 0a0a 215b 4669 6c69 6e67 7320 696e  ``..![Filings in
-000033f0: 2032 3032 315d 2868 7474 7073 3a2f 2f72   2021](https://r
-00003400: 6177 2e67 6974 6875 6275 7365 7263 6f6e  aw.githubusercon
-00003410: 7465 6e74 2e63 6f6d 2f64 6775 6e6e 696e  tent.com/dgunnin
-00003420: 672f 6564 6761 7274 6f6f 6c73 2f6d 6169  g/edgartools/mai
-00003430: 6e2f 6669 6c69 6e67 735f 3230 3231 2e6a  n/filings_2021.j
-00003440: 7067 290a 0a23 2323 2320 4765 7420 6669  pg)..#### Get fi
-00003450: 6c69 6e67 7320 666f 7220 3230 3231 2071  lings for 2021 q
-00003460: 7561 7274 6572 2034 0a49 6e73 7465 6164  uarter 4.Instead
-00003470: 206f 6620 6765 7474 696e 6720 7468 6520   of getting the 
-00003480: 6669 6c69 6e67 7320 666f 7220 616e 2065  filings for an e
-00003490: 6e74 6972 6520 7965 6172 2c20 796f 7520  ntire year, you 
-000034a0: 6361 6e20 6765 7420 7468 6520 6669 6c69  can get the fili
-000034b0: 6e67 7320 666f 7220 6120 7175 6172 7465  ngs for a quarte
-000034c0: 722e 0a60 6060 7079 7468 6f6e 0a66 696c  r..```python.fil
-000034d0: 696e 6773 203d 2067 6574 5f66 696c 696e  ings = get_filin
-000034e0: 6773 2832 3032 312c 2034 290a 6060 600a  gs(2021, 4).```.
-000034f0: 0a23 2323 2320 4765 7420 6669 6c69 6e67  .#### Get filing
-00003500: 7320 6265 7477 6565 6e20 3230 3130 2061  s between 2010 a
-00003510: 6e64 2032 3031 390a 596f 7520 6361 6e20  nd 2019.You can 
-00003520: 6765 7420 7468 6520 6669 6c69 6e67 7320  get the filings 
-00003530: 666f 7220 6120 7261 6e67 6520 6f66 2079  for a range of y
-00003540: 6561 7273 2c20 7369 6e63 6520 7468 6520  ears, since the 
-00003550: 6079 6561 7260 2070 6172 616d 6574 6572  `year` parameter
-00003560: 2061 6363 6570 7473 2061 2076 616c 7565   accepts a value
-00003570: 2c20 6120 6c69 7374 206f 7220 6120 7261  , a list or a ra
-00003580: 6e67 652e 0a60 6060 7079 7468 6f6e 0a66  nge..```python.f
-00003590: 696c 696e 6773 203d 2067 6574 5f66 696c  ilings = get_fil
-000035a0: 696e 6773 2872 616e 6765 2832 3031 302c  ings(range(2010,
-000035b0: 2032 3032 3029 290a 6060 600a 0a23 2323   2020)).```..###
-000035c0: 2320 4765 7420 5842 524c 2066 696c 696e  # Get XBRL filin
-000035d0: 6773 2066 6f72 2032 3032 320a 6060 6070  gs for 2022.```p
-000035e0: 7974 686f 6e0a 6669 6c69 6e67 7320 3d20  ython.filings = 
-000035f0: 6765 745f 6669 6c69 6e67 7328 3230 3232  get_filings(2022
-00003600: 2c20 696e 6465 783d 2278 6272 6c22 290a  , index="xbrl").
-00003610: 6060 600a 0a0a 2323 2323 2046 696c 7465  ```...#### Filte
-00003620: 7269 6e67 2046 696c 696e 6773 2062 7920  ring Filings by 
-00003630: 666f 726d 0a59 6f75 2063 616e 2066 696c  form.You can fil
-00003640: 7465 7220 6279 2066 6f72 6d20 7479 7065  ter by form type
-00003650: 2062 7920 7072 6f76 6964 696e 6720 6120   by providing a 
-00003660: 666f 726d 206f 7220 6c69 7374 206f 6620  form or list of 
-00003670: 666f 726d 732e 0a60 6060 7079 7468 6f6e  forms..```python
-00003680: 0a66 696c 696e 6773 203d 2067 6574 5f66  .filings = get_f
-00003690: 696c 696e 6773 2832 3032 322c 2066 6f72  ilings(2022, for
-000036a0: 6d3d 2231 302d 4b22 290a 0a23 2046 696c  m="10-K")..# Fil
-000036b0: 7465 7220 6279 206c 6973 7420 6f66 2066  ter by list of f
-000036c0: 6f72 6d73 0a66 696c 696e 6773 203d 2067  orms.filings = g
-000036d0: 6574 5f66 696c 696e 6773 2832 3032 322c  et_filings(2022,
-000036e0: 2066 6f72 6d3d 5b22 3130 2d4b 222c 2022   form=["10-K", "
-000036f0: 3130 2d51 225d 290a 6060 600a 0a54 6869  10-Q"]).```..Thi
-00003700: 7320 7769 6c6c 2069 6e63 6c75 6465 2066  s will include f
-00003710: 6f72 6d20 616d 656e 646d 656e 7473 2065  orm amendments e
-00003720: 2e67 2e20 2231 302d 4b2f 4122 2061 6e64  .g. "10-K/A" and
-00003730: 2022 3130 2d51 2f41 222e 2054 6f20 6e6f   "10-Q/A". To no
-00003740: 7420 696e 636c 7564 6520 7468 6573 6520  t include these 
-00003750: 7365 7420 6061 6d65 6e64 6d65 6e74 733d  set `amendments=
-00003760: 4661 6c73 6560 0a60 6060 7079 7468 6f6e  False`.```python
-00003770: 0a23 2046 696c 7465 7220 6279 206c 6973  .# Filter by lis
-00003780: 7420 6f66 2066 6f72 6d73 206e 6f74 2069  t of forms not i
-00003790: 6e63 6c75 6469 6e67 2061 6d65 6e64 6d65  ncluding amendme
-000037a0: 6e74 730a 6669 6c69 6e67 7320 3d20 6765  nts.filings = ge
-000037b0: 745f 6669 6c69 6e67 7328 3230 3232 2c20  t_filings(2022, 
-000037c0: 666f 726d 3d5b 2231 302d 4b22 2c20 2231  form=["10-K", "1
-000037d0: 302d 5122 5d2c 2061 6d65 6e64 6d65 6e74  0-Q"], amendment
-000037e0: 733d 4661 6c73 6529 0a60 6060 0a0a 2323  s=False).```..##
-000037f0: 2320 5468 6520 4669 6c69 6e67 7320 636c  # The Filings cl
-00003800: 6173 730a 0a54 6865 2060 6765 745f 6669  ass..The `get_fi
-00003810: 6c69 6e67 7360 2072 6574 7572 6e73 2061  lings` returns a
-00003820: 2060 4669 6c69 6e67 7360 2063 6c61 7373   `Filings` class
-00003830: 2c20 7768 6963 6820 7772 6170 7320 7468  , which wraps th
-00003840: 6520 6461 7461 2072 6574 7572 6e65 6420  e data returned 
-00003850: 616e 6420 7072 6f76 6964 6520 636f 6e76  and provide conv
-00003860: 656e 6965 6e74 2077 6179 7320 666f 7220  enient ways for 
-00003870: 776f 726b 696e 6720 7769 7468 2066 696c  working with fil
-00003880: 696e 6773 2e0a 0a23 2323 2320 436f 6e76  ings...#### Conv
-00003890: 6572 7420 7468 6520 6669 6c69 6e67 7320  ert the filings 
-000038a0: 746f 2061 2070 616e 6461 7320 6461 7461  to a pandas data
-000038b0: 6672 616d 650a 0a54 6865 2066 696c 696e  frame..The filin
-000038c0: 6773 2064 6174 6120 6973 2073 746f 7265  gs data is store
-000038d0: 6420 696e 2074 6865 2060 4669 6c69 6e67  d in the `Filing
-000038e0: 7360 2063 6c61 7373 2061 7320 6120 6070  s` class as a `p
-000038f0: 7961 7272 6f77 2e54 6162 6c65 602e 2059  yarrow.Table`. Y
-00003900: 6f75 2063 616e 2067 6574 2074 6865 2064  ou can get the d
-00003910: 6174 6120 6173 2061 2070 616e 6461 7320  ata as a pandas 
-00003920: 6461 7461 6672 616d 6520 7573 696e 670a  dataframe using.
-00003930: 6074 6f5f 7061 6e64 6173 600a 6060 6070  `to_pandas`.```p
-00003940: 7974 686f 6e0a 6466 203d 2066 696c 696e  ython.df = filin
-00003950: 6773 2e74 6f5f 7061 6e64 6173 2829 0a60  gs.to_pandas().`
-00003960: 6060 0a0a 2323 2057 6f72 6b69 6e67 2077  ``..## Working w
-00003970: 6974 6820 616e 2069 6e64 6976 6964 7561  ith an individua
-00003980: 6c20 4669 6c69 6e67 0a0a 4f6e 6365 2079  l Filing..Once y
-00003990: 6f75 2068 6176 6520 7265 7472 6965 7665  ou have retrieve
-000039a0: 6420 4669 6c69 6e67 7320 796f 7520 6361  d Filings you ca
-000039b0: 6e20 6163 6365 7373 2069 6e64 6976 6964  n access individ
-000039c0: 7561 6c20 6669 6c69 6e67 7320 7573 696e  ual filings usin
-000039d0: 6720 7468 6520 6272 6163 6b65 7420 605b  g the bracket `[
-000039e0: 5d60 206e 6f74 6174 696f 6e2e 0a60 6060  ]` notation..```
-000039f0: 7079 7468 6f6e 0a66 696c 696e 6773 203d  python.filings =
-00003a00: 2067 6574 5f66 696c 696e 6773 2832 3032   get_filings(202
-00003a10: 3129 0a66 696c 696e 6720 3d20 6669 6c69  1).filing = fili
-00003a20: 6e67 735b 305d 0a60 6060 0a21 5b46 696c  ngs[0].```.![Fil
-00003a30: 696e 6773 2069 6e20 3230 3231 5d28 6874  ings in 2021](ht
-00003a40: 7470 733a 2f2f 7261 772e 6769 7468 7562  tps://raw.github
-00003a50: 7573 6572 636f 6e74 656e 742e 636f 6d2f  usercontent.com/
-00003a60: 6467 756e 6e69 6e67 2f65 6467 6172 746f  dgunning/edgarto
-00003a70: 6f6c 732f 6d61 696e 2f66 696c 696e 6773  ols/main/filings
-00003a80: 5f32 3032 312e 6a70 6729 0a50 6179 2061  _2021.jpg).Pay a
-00003a90: 7474 656e 7469 6f6e 2074 6f20 7468 6520  ttention to the 
-00003aa0: 696e 6465 7820 7661 6c75 6520 6469 7370  index value disp
-00003ab0: 6c61 7965 6420 666f 7220 7468 6520 6669  layed for the fi
-00003ac0: 6c69 6e67 732e 2054 6869 7320 6973 2074  lings. This is t
-00003ad0: 6865 2076 616c 7565 2079 6f75 200a 7769  he value you .wi
-00003ae0: 6c6c 2075 7365 2074 6f20 6765 7420 7468  ll use to get th
-00003af0: 6520 696e 6469 7669 6475 616c 2066 696c  e individual fil
-00003b00: 696e 672e 0a60 6060 7079 7468 6f6e 0a66  ing..```python.f
-00003b10: 696c 696e 6720 3d20 6669 6c69 6e67 735b  iling = filings[
-00003b20: 305d 0a60 6060 0a21 5b41 2073 696e 676c  0].```.![A singl
-00003b30: 6520 6669 6c69 6e67 5d28 6874 7470 733a  e filing](https:
-00003b40: 2f2f 7261 772e 6769 7468 7562 7573 6572  //raw.githubuser
-00003b50: 636f 6e74 656e 742e 636f 6d2f 6467 756e  content.com/dgun
-00003b60: 6e69 6e67 2f65 6467 6172 746f 6f6c 732f  ning/edgartools/
-00003b70: 6d61 696e 2f73 696e 676c 655f 6669 6c69  main/single_fili
-00003b80: 6e67 2e70 6e67 290a 0a23 2323 204f 7065  ng.png)..### Ope
-00003b90: 6e20 6120 6669 6c69 6e67 0a0a 596f 7520  n a filing..You 
-00003ba0: 6361 6e20 6f70 656e 2074 6865 2066 696c  can open the fil
-00003bb0: 696e 6720 696e 2079 6f75 7220 6272 6f77  ing in your brow
-00003bc0: 7365 7220 7573 696e 6720 6066 696c 696e  ser using `filin
-00003bd0: 672e 6f70 656e 2829 600a 6060 6070 7974  g.open()`.```pyt
-00003be0: 686f 6e0a 6669 6c69 6e67 2e6f 7065 6e28  hon.filing.open(
-00003bf0: 290a 6060 600a 0a23 2323 204f 7065 6e20  ).```..### Open 
-00003c00: 7468 6520 4669 6c69 6e67 2048 6f6d 6570  the Filing Homep
-00003c10: 6167 650a 596f 7520 6361 6e20 6f70 656e  age.You can open
-00003c20: 2074 6865 2066 696c 696e 6720 686f 6d65   the filing home
-00003c30: 7061 6765 2069 6e20 7468 6520 6272 6f77  page in the brow
-00003c40: 7365 7220 7573 696e 6720 6066 696c 696e  ser using `filin
-00003c50: 672e 6f70 656e 5f68 6f6d 6570 6167 6528  g.open_homepage(
-00003c60: 2960 0a60 6060 7079 7468 6f6e 0a66 696c  )`.```python.fil
-00003c70: 696e 672e 6f70 656e 2829 0a60 6060 0a0a  ing.open().```..
-00003c80: 0a23 2323 2320 5573 6520 4475 636b 4442  .#### Use DuckDB
-00003c90: 2074 6f20 7175 6572 7920 7468 6520 6669   to query the fi
-00003ca0: 6c69 6e67 730a 0a41 2063 6f6e 7665 6965  lings..A conveie
-00003cb0: 6e74 2077 6179 2074 6f20 7175 6572 7920  nt way to query 
-00003cc0: 7468 6520 6669 6c69 6e67 7320 6461 7461  the filings data
-00003cd0: 2069 7320 746f 2075 7365 202a 2a44 7563   is to use **Duc
-00003ce0: 6b44 422a 2a2e 2049 6620 796f 7520 6361  kDB**. If you ca
-00003cf0: 6c6c 2074 6865 2060 746f 5f64 7563 6b64  ll the `to_duckd
-00003d00: 6260 2066 756e 6374 696f 6e2c 2079 6f75  b` function, you
-00003d10: 2067 6574 2061 6e20 696e 2d6d 656d 6f72   get an in-memor
-00003d20: 790a 4475 636b 4442 2064 6174 6162 6173  y.DuckDB databas
-00003d30: 6520 696e 7374 616e 6365 2c20 7769 7468  e instance, with
-00003d40: 2074 6865 2066 696c 696e 6773 2072 6567   the filings reg
-00003d50: 6973 7465 7265 6420 6173 2061 2074 6162  istered as a tab
-00003d60: 6c65 2063 616c 6c65 6420 6066 696c 696e  le called `filin
-00003d70: 6773 602e 0a54 6865 6e20 796f 7520 6361  gs`..Then you ca
-00003d80: 6e20 776f 726b 2064 6972 6563 7479 2077  n work directy w
-00003d90: 6974 6820 7468 6520 4475 636b 4442 2064  ith the DuckDB d
-00003da0: 6174 6162 6173 652c 2061 6e64 2072 756e  atabase, and run
-00003db0: 2053 514c 2061 6761 696e 7374 2074 6865   SQL against the
-00003dc0: 2066 696c 696e 6773 2064 6174 612e 0a0a   filings data...
-00003dd0: 496e 2074 6869 7320 6578 616d 706c 652c  In this example,
-00003de0: 2077 6520 6669 6c74 6572 2066 696c 696e   we filter filin
-00003df0: 6773 2066 6f72 202a 2a53 2d31 2a2a 2066  gs for **S-1** f
-00003e00: 6f72 6d20 7479 7065 732e 0a0a 6060 6070  orm types...```p
-00003e10: 7974 686f 6e0a 6462 203d 2066 696c 696e  ython.db = filin
-00003e20: 6773 2e74 6f5f 6475 636b 6462 2829 0a23  gs.to_duckdb().#
-00003e30: 2061 2064 7563 6b64 622e 4475 636b 4442   a duckdb.DuckDB
-00003e40: 5079 436f 6e6e 6563 7469 6f6e 0a0a 2320  PyConnection..# 
-00003e50: 5175 6572 7920 7468 6520 6669 6c69 6e67  Query the filing
-00003e60: 7320 666f 7220 532d 3120 6669 6c69 6e67  s for S-1 filing
-00003e70: 7320 616e 6420 7265 7475 726e 2061 2064  s and return a d
-00003e80: 6174 6166 7261 6d65 0a64 622e 6578 6563  ataframe.db.exec
-00003e90: 7574 6528 2222 220a 7365 6c65 6374 202a  ute(""".select *
-00003ea0: 2066 726f 6d20 6669 6c69 6e67 7320 7768   from filings wh
-00003eb0: 6572 6520 466f 726d 203d 3d20 2753 2d31  ere Form == 'S-1
-00003ec0: 270a 2222 2229 2e64 6628 290a 6060 600a  '.""").df().```.
-00003ed0: 0a23 2043 6f6e 7472 6962 7574 696e 670a  .# Contributing.
-00003ee0: 0a43 6f6e 7472 6962 7574 696f 6e73 2061  .Contributions a
-00003ef0: 7265 2077 656c 636f 6d65 2120 5765 2077  re welcome! We w
-00003f00: 6f75 6c64 206c 6f76 6520 746f 2068 6561  ould love to hea
-00003f10: 7220 796f 7572 2074 686f 7567 6874 7320  r your thoughts 
-00003f20: 6f6e 2068 6f77 2074 6869 7320 6c69 6272  on how this libr
-00003f30: 6172 7920 636f 756c 6420 6265 2062 6574  ary could be bet
-00003f40: 7465 7220 6174 2077 6f72 6b69 6e67 2077  ter at working w
-00003f50: 6974 6820 5345 4320 4564 6761 722e 0a0a  ith SEC Edgar...
-00003f60: 2323 2052 6570 6f72 7469 6e67 2049 7373  ## Reporting Iss
-00003f70: 7565 730a 5765 2075 7365 2047 6974 4875  ues.We use GitHu
-00003f80: 6220 6973 7375 6573 2074 6f20 7472 6163  b issues to trac
-00003f90: 6b20 7075 626c 6963 2062 7567 732e 200a  k public bugs. .
-00003fa0: 5265 706f 7274 2061 2062 7567 2062 7920  Report a bug by 
-00003fb0: 5b6f 7065 6e69 6e67 2061 206e 6577 2069  [opening a new i
-00003fc0: 7373 7565 5d28 6874 7470 733a 2f2f 6769  ssue](https://gi
-00003fd0: 7468 7562 2e63 6f6d 2f64 6775 6e6e 696e  thub.com/dgunnin
-00003fe0: 672f 6564 6761 7274 6f6f 6c73 2f69 7373  g/edgartools/iss
-00003ff0: 7565 7329 3b20 6974 2773 2074 6861 7420  ues); it's that 
-00004000: 6561 7379 210a 0a23 2320 4d61 6b69 6e67  easy!..## Making
-00004010: 2063 6f64 6520 6368 616e 6765 730a 2d20   code changes.- 
-00004020: 466f 726b 2074 6865 2072 6570 6f20 616e  Fork the repo an
-00004030: 6420 6372 6561 7465 2079 6f75 7220 6272  d create your br
-00004040: 616e 6368 2066 726f 6d20 6d61 7374 6572  anch from master
-00004050: 2e0a 2d20 4966 2079 6f75 2776 6520 6164  ..- If you've ad
-00004060: 6465 6420 636f 6465 2074 6861 7420 7368  ded code that sh
-00004070: 6f75 6c64 2062 6520 7465 7374 6564 2c20  ould be tested, 
-00004080: 6164 6420 7465 7374 732e 0a2d 2049 6620  add tests..- If 
-00004090: 796f 7527 7665 2063 6861 6e67 6564 2041  you've changed A
-000040a0: 5049 732c 2075 7064 6174 6520 7468 6520  PIs, update the 
-000040b0: 646f 6375 6d65 6e74 6174 696f 6e2e 0a2d  documentation..-
-000040c0: 2045 6e73 7572 6520 7468 6520 7465 7374   Ensure the test
-000040d0: 2073 7569 7465 2070 6173 7365 732e 0a2d   suite passes..-
-000040e0: 204d 616b 6520 7375 7265 2079 6f75 7220   Make sure your 
-000040f0: 636f 6465 206c 696e 7473 2e0a 2d20 4973  code lints..- Is
-00004100: 7375 6520 7468 6174 2070 756c 6c20 7265  sue that pull re
-00004110: 7175 6573 7421 0a0a 0a0a 2320 4c69 6365  quest!....# Lice
-00004120: 6e73 650a 0a60 6564 6761 7274 6f6f 6c73  nse..`edgartools
-00004130: 6020 6973 2064 6973 7472 6962 7574 6564  ` is distributed
-00004140: 2075 6e64 6572 2074 6865 2074 6572 6d73   under the terms
-00004150: 206f 6620 7468 6520 5b4d 4954 5d28 6874   of the [MIT](ht
-00004160: 7470 733a 2f2f 7370 6478 2e6f 7267 2f6c  tps://spdx.org/l
-00004170: 6963 656e 7365 732f 4d49 542e 6874 6d6c  icenses/MIT.html
-00004180: 2920 6c69 6365 6e73 652e 0a0a 2323 2043  ) license...## C
-00004190: 6f6e 7461 6374 0a0a 5b4c 696e 6b65 6449  ontact..[LinkedI
-000041a0: 6e5d 2868 7474 7073 3a2f 2f77 7777 2e6c  n](https://www.l
-000041b0: 696e 6b65 6469 6e2e 636f 6d2f 696e 2f64  inkedin.com/in/d
-000041c0: 7769 6768 742d 6775 6e6e 696e 672d 3836  wight-gunning-86
-000041d0: 3031 3234 2f29                           0124/)
+00000560: 6e2f 696d 6167 6573 2f65 6467 6172 2d74  n/images/edgar-t
+00000570: 6f6f 6c73 2e70 6e67 290a 0a5b 215b 5079  ools.png)..[![Py
+00000580: 5049 202d 2056 6572 7369 6f6e 5d28 6874  PI - Version](ht
+00000590: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
+000005a0: 732e 696f 2f70 7970 692f 762f 6564 6761  s.io/pypi/v/edga
+000005b0: 7274 6f6f 6c73 2e73 7667 295d 2868 7474  rtools.svg)](htt
+000005c0: 7073 3a2f 2f70 7970 692e 6f72 672f 7072  ps://pypi.org/pr
+000005d0: 6f6a 6563 742f 6564 6761 7274 6f6f 6c73  oject/edgartools
+000005e0: 290a 215b 4769 7448 7562 206c 6173 7420  ).![GitHub last 
+000005f0: 636f 6d6d 6974 5d28 6874 7470 733a 2f2f  commit](https://
+00000600: 696d 672e 7368 6965 6c64 732e 696f 2f67  img.shields.io/g
+00000610: 6974 6875 622f 6c61 7374 2d63 6f6d 6d69  ithub/last-commi
+00000620: 742f 6467 756e 6e69 6e67 2f65 6467 6172  t/dgunning/edgar
+00000630: 746f 6f6c 7329 0a21 5b47 6974 4875 6220  tools).![GitHub 
+00000640: 576f 726b 666c 6f77 2053 7461 7475 735d  Workflow Status]
+00000650: 2868 7474 7073 3a2f 2f69 6d67 2e73 6869  (https://img.shi
+00000660: 656c 6473 2e69 6f2f 6769 7468 7562 2f61  elds.io/github/a
+00000670: 6374 696f 6e73 2f77 6f72 6b66 6c6f 772f  ctions/workflow/
+00000680: 7374 6174 7573 2f64 6775 6e6e 696e 672f  status/dgunning/
+00000690: 6564 6761 7274 6f6f 6c73 2f70 7974 686f  edgartools/pytho
+000006a0: 6e2d 6861 7463 682d 776f 726b 666c 6f77  n-hatch-workflow
+000006b0: 2e79 6d6c 290a 5b21 5b43 6f64 6546 6163  .yml).[![CodeFac
+000006c0: 746f 725d 2868 7474 7073 3a2f 2f77 7777  tor](https://www
+000006d0: 2e63 6f64 6566 6163 746f 722e 696f 2f72  .codefactor.io/r
+000006e0: 6570 6f73 6974 6f72 792f 6769 7468 7562  epository/github
+000006f0: 2f64 6775 6e6e 696e 672f 6564 6761 7274  /dgunning/edgart
+00000700: 6f6f 6c73 2f62 6164 6765 295d 2868 7474  ools/badge)](htt
+00000710: 7073 3a2f 2f77 7777 2e63 6f64 6566 6163  ps://www.codefac
+00000720: 746f 722e 696f 2f72 6570 6f73 6974 6f72  tor.io/repositor
+00000730: 792f 6769 7468 7562 2f64 6775 6e6e 696e  y/github/dgunnin
+00000740: 672f 6564 6761 7274 6f6f 6c73 290a 5b21  g/edgartools).[!
+00000750: 5b48 6174 6368 2070 726f 6a65 6374 5d28  [Hatch project](
+00000760: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
+00000770: 6c64 732e 696f 2f62 6164 6765 2f25 4630  lds.io/badge/%F0
+00000780: 2539 4625 4135 2539 412d 4861 7463 682d  %9F%A5%9A-Hatch-
+00000790: 3430 3531 6235 2e73 7667 295d 2868 7474  4051b5.svg)](htt
+000007a0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+000007b0: 7079 7061 2f68 6174 6368 290a 215b 4769  pypa/hatch).![Gi
+000007c0: 7448 7562 5d28 6874 7470 733a 2f2f 696d  tHub](https://im
+000007d0: 672e 7368 6965 6c64 732e 696f 2f67 6974  g.shields.io/git
+000007e0: 6875 622f 6c69 6365 6e73 652f 6467 756e  hub/license/dgun
+000007f0: 6e69 6e67 2f65 6467 6172 746f 6f6c 7329  ning/edgartools)
+00000800: 0a2d 2d2d 2d2d 0a0a 3c21 2d2d 2054 4142  .-----..<!-- TAB
+00000810: 4c45 204f 4620 434f 4e54 454e 5453 202d  LE OF CONTENTS -
+00000820: 2d3e 0a3c 6465 7461 696c 733e 0a20 203c  ->.<details>.  <
+00000830: 7375 6d6d 6172 793e 5461 626c 6520 6f66  summary>Table of
+00000840: 2043 6f6e 7465 6e74 733c 2f73 756d 6d61   Contents</summa
+00000850: 7279 3e0a 2020 3c6f 6c3e 0a20 2020 203c  ry>.  <ol>.    <
+00000860: 6c69 3e0a 2020 2020 2020 3c61 2068 7265  li>.      <a hre
+00000870: 663d 2223 6162 6f75 742d 7468 652d 7072  f="#about-the-pr
+00000880: 6f6a 6563 7422 3e41 626f 7574 2054 6865  oject">About The
+00000890: 2050 726f 6a65 6374 3c2f 613e 0a20 2020   Project</a>.   
+000008a0: 2020 203c 756c 3e0a 2020 2020 2020 2020     <ul>.        
+000008b0: 3c6c 693e 3c61 2068 7265 663d 2223 6465  <li><a href="#de
+000008c0: 6d6f 223e 4465 6d6f 3c2f 613e 3c2f 6c69  mo">Demo</a></li
+000008d0: 3e0a 2020 2020 2020 2020 3c6c 693e 3c61  >.        <li><a
+000008e0: 2068 7265 663d 2223 6665 6174 7572 6573   href="#features
+000008f0: 223e 4665 6174 7572 6573 3c2f 613e 3c2f  ">Features</a></
+00000900: 6c69 3e0a 2020 2020 2020 3c2f 756c 3e0a  li>.      </ul>.
+00000910: 2020 2020 3c2f 6c69 3e0a 2020 2020 3c6c      </li>.    <l
+00000920: 693e 0a20 2020 2020 2020 203c 6120 6872  i>.        <a hr
+00000930: 6566 3d22 2369 6e73 7461 6c6c 6174 696f  ef="#installatio
+00000940: 6e22 3e49 6e73 7461 6c6c 6174 696f 6e3c  n">Installation<
+00000950: 2f61 3e0a 2020 2020 3c2f 6c69 3e0a 2020  /a>.    </li>.  
+00000960: 2020 3c6c 693e 0a20 2020 2020 2020 203c    <li>.        <
+00000970: 6120 6872 6566 3d22 2375 7361 6765 223e  a href="#usage">
+00000980: 5573 6167 653c 2f61 3e0a 2020 2020 2020  Usage</a>.      
+00000990: 2020 3c75 6c3e 0a20 2020 2020 2020 2020    <ul>.         
+000009a0: 2020 203c 6c69 3e3c 6120 6872 6566 3d22     <li><a href="
+000009b0: 2373 6574 7469 6e67 2d79 6f75 722d 6564  #setting-your-ed
+000009c0: 6761 722d 7573 6572 2d69 6465 6e74 6974  gar-user-identit
+000009d0: 7922 3e53 6574 7469 6e67 2079 6f75 7220  y">Setting your 
+000009e0: 4564 6761 7220 7573 6572 2069 6465 6e74  Edgar user ident
+000009f0: 6974 793c 2f61 3e3c 2f6c 693e 0a20 2020  ity</a></li>.   
+00000a00: 2020 2020 2020 2020 203c 6c69 3e3c 6120           <li><a 
+00000a10: 6872 6566 3d22 2367 6574 7469 6e67 2d66  href="#getting-f
+00000a20: 696c 696e 6773 223e 4765 7474 696e 6720  ilings">Getting 
+00000a30: 4669 6c69 6e67 733c 2f61 3e3c 2f6c 693e  Filings</a></li>
+00000a40: 0a20 2020 2020 2020 2020 2020 203c 6c69  .            <li
+00000a50: 3e3c 6120 6872 6566 3d22 2375 7369 6e67  ><a href="#using
+00000a60: 2d74 6865 2d63 6f6d 7061 6e79 2d61 7069  -the-company-api
+00000a70: 223e 5573 696e 6720 7468 6520 436f 6d70  ">Using the Comp
+00000a80: 616e 7920 4150 493c 2f61 3e3c 2f6c 693e  any API</a></li>
+00000a90: 0a20 2020 2020 203c 2f75 6c3e 0a20 2020  .      </ul>.   
+00000aa0: 203c 2f6c 693e 0a20 2020 203c 6c69 3e3c   </li>.    <li><
+00000ab0: 6120 6872 6566 3d22 2363 6f6e 7472 6962  a href="#contrib
+00000ac0: 7574 696e 6722 3e43 6f6e 7472 6962 7574  uting">Contribut
+00000ad0: 696e 673c 2f61 3e3c 2f6c 693e 0a20 2020  ing</a></li>.   
+00000ae0: 203c 6c69 3e3c 6120 6872 6566 3d22 236c   <li><a href="#l
+00000af0: 6963 656e 7365 223e 4c69 6365 6e73 653c  icense">License<
+00000b00: 2f61 3e3c 2f6c 693e 0a20 2020 203c 6c69  /a></li>.    <li
+00000b10: 3e3c 6120 6872 6566 3d22 2363 6f6e 7461  ><a href="#conta
+00000b20: 6374 223e 436f 6e74 6163 743c 2f61 3e3c  ct">Contact</a><
+00000b30: 2f6c 693e 0a20 203c 2f6f 6c3e 0a3c 2f64  /li>.  </ol>.</d
+00000b40: 6574 6169 6c73 3e0a 0a23 2041 626f 7574  etails>..# About
+00000b50: 2074 6865 2070 726f 6a65 6374 0a0a 2a2a   the project..**
+00000b60: 6065 6467 6172 746f 6f6c 7360 2a2a 2069  `edgartools`** i
+00000b70: 7320 6120 6c69 6272 6172 7920 666f 7220  s a library for 
+00000b80: 776f 726b 696e 6720 7769 7468 2053 4543  working with SEC
+00000b90: 2045 6467 6172 2066 696c 696e 6773 2e20   Edgar filings. 
+00000ba0: 596f 7520 6361 6e20 7175 6572 792c 2066  You can query, f
+00000bb0: 696c 7465 7220 616e 6420 7365 6c65 6374  ilter and select
+00000bc0: 2061 6e79 2066 696c 696e 6720 7369 6e63   any filing sinc
+00000bd0: 6520 3139 3934 2061 6e64 2076 6965 7720  e 1994 and view 
+00000be0: 7468 6520 6669 6c69 6e67 2773 2068 746d  the filing's htm
+00000bf0: 6c2c 2074 6578 742c 2078 6d6c 206f 7220  l, text, xml or 
+00000c00: 7374 7275 6374 7572 6564 2064 6174 612e  structured data.
+00000c10: 0a0a 0a23 2320 4465 6d6f 0a0a 2323 2323  ...## Demo..####
+00000c20: 2047 6574 2074 6865 2043 6f6d 6d6f 6e20   Get the Common 
+00000c30: 5368 6172 6573 2049 7373 7565 6420 616d  Shares Issued am
+00000c40: 6f75 6e74 2066 726f 6d20 536e 6f77 666c  ount from Snowfl
+00000c50: 616b 6527 7320 6c61 7465 7374 2031 302d  ake's latest 10-
+00000c60: 5120 6669 6c69 6e67 0a0a 6060 6070 7974  Q filing..```pyt
+00000c70: 686f 6e0a 2843 6f6d 7061 6e79 2822 534e  hon.(Company("SN
+00000c80: 4f57 2229 0a20 2020 2020 2020 202e 6765  OW").        .ge
+00000c90: 745f 6669 6c69 6e67 7328 666f 726d 3d22  t_filings(form="
+00000ca0: 3130 2d51 2229 0a20 2020 2020 2020 202e  10-Q").        .
+00000cb0: 6c61 7465 7374 2829 0a20 2020 2020 2020  latest().       
+00000cc0: 202e 7862 726c 2829 0a20 2020 2020 2020   .xbrl().       
+00000cd0: 202e 746f 5f64 7563 6b64 6228 292e 6578   .to_duckdb().ex
+00000ce0: 6563 7574 6528 0a20 2020 2020 2020 2022  ecute(.        "
+00000cf0: 2222 7365 6c65 6374 2066 6163 742c 2076  ""select fact, v
+00000d00: 616c 7565 2c20 756e 6974 732c 2065 6e64  alue, units, end
+00000d10: 5f64 6174 6520 6672 6f6d 2066 6163 7473  _date from facts
+00000d20: 200a 2020 2020 2020 2020 2020 2077 6865   .           whe
+00000d30: 7265 2066 6163 7420 3d20 2743 6f6d 6d6f  re fact = 'Commo
+00000d40: 6e53 746f 636b 5368 6172 6573 4973 7375  nStockSharesIssu
+00000d50: 6564 2720 0a20 2020 2020 2020 2020 2020  ed' .           
+00000d60: 6f72 6465 7220 6279 2065 6e64 5f64 6174  order by end_dat
+00000d70: 6520 6465 7363 206c 696d 6974 2031 0a20  e desc limit 1. 
+00000d80: 2020 2020 2020 2022 2222 0a20 2020 2029         """.    )
+00000d90: 2e64 6628 290a 290a 6060 600a 0a21 5b43  .df().).```..![C
+00000da0: 6f6d 6d6f 6e20 5368 6172 6573 2049 7373  ommon Shares Iss
+00000db0: 7565 645d 2868 7474 7073 3a2f 2f72 6177  ued](https://raw
+00000dc0: 2e67 6974 6875 6275 7365 7263 6f6e 7465  .githubuserconte
+00000dd0: 6e74 2e63 6f6d 2f64 6775 6e6e 696e 672f  nt.com/dgunning/
+00000de0: 6564 6761 7274 6f6f 6c73 2f6d 6169 6e2f  edgartools/main/
+00000df0: 696d 6167 6573 2f63 6f6d 6d6f 6e2d 7368  images/common-sh
+00000e00: 6172 6573 2d69 7373 7565 642e 706e 6729  ares-issued.png)
+00000e10: 0a0a 5468 6973 2065 7861 6d70 6c65 2073  ..This example s
+00000e20: 686f 7773 2077 6861 7420 6361 6e20 6265  hows what can be
+00000e30: 2064 6f6e 6520 7769 7468 202a 2a65 6467   done with **edg
+00000e40: 6172 746f 6f6c 732a 2a2e 0a0a 556e 6465  artools**...Unde
+00000e50: 7220 7468 6520 686f 6f64 2074 6865 2063  r the hood the c
+00000e60: 6f64 6520 646f 6573 2074 6865 2066 6f6c  ode does the fol
+00000e70: 6c6f 7769 6e67 0a0a 312e 2055 7365 2074  lowing..1. Use t
+00000e80: 6865 2074 6963 6b65 7220 2a2a 2253 4e4f  he ticker **"SNO
+00000e90: 5722 2a2a 2074 6f20 6765 7420 7468 6520  W"** to get the 
+00000ea0: 636f 6d70 616e 7927 7320 6369 6b20 6672  company's cik fr
+00000eb0: 6f6d 2074 6865 205b 436f 6d70 616e 7920  om the [Company 
+00000ec0: 5469 636b 6572 7320 4a53 4f4e 5d28 6874  Tickers JSON](ht
+00000ed0: 7470 733a 2f2f 7777 772e 7365 632e 676f  tps://www.sec.go
+00000ee0: 762f 6669 6c65 2f63 6f6d 7061 6e79 2d74  v/file/company-t
+00000ef0: 6963 6b65 7273 290a 322e 2046 726f 6d20  ickers).2. From 
+00000f00: 7468 6520 2a2a 6369 6b2a 2a20 6765 7420  the **cik** get 
+00000f10: 7468 6520 636f 6d70 616e 7927 7320 6669  the company's fi
+00000f20: 6c69 6e67 7320 6672 6f6d 2074 6865 2073  lings from the s
+00000f30: 7562 6d69 7373 696f 6e73 2065 6e64 706f  ubmissions endpo
+00000f40: 696e 7420 6068 7474 7073 3a2f 2f64 6174  int `https://dat
+00000f50: 612e 7365 632e 676f 762f 7375 626d 6973  a.sec.gov/submis
+00000f60: 7369 6f6e 732f 4349 4b7b 6369 6b3a 3031  sions/CIK{cik:01
+00000f70: 307d 2e6a 736f 6e60 0a33 2e20 5365 6c65  0}.json`.3. Sele
+00000f80: 6374 2074 6865 206c 6174 6573 7420 3130  ct the latest 10
+00000f90: 2d51 2066 696c 696e 670a 342e 2044 6f77  -Q filing.4. Dow
+00000fa0: 6e6c 6f61 6420 7468 6520 5842 524c 2066  nload the XBRL f
+00000fb0: 696c 6520 666f 7220 7468 6174 2066 696c  ile for that fil
+00000fc0: 696e 670a 352e 2043 6f6e 7665 7274 2074  ing.5. Convert t
+00000fd0: 6865 2058 4252 4c20 6461 7461 2069 6e74  he XBRL data int
+00000fe0: 6f20 6120 7061 6e64 6173 2064 6174 6166  o a pandas dataf
+00000ff0: 7261 6d65 0a36 2e20 5265 6769 7374 6572  rame.6. Register
+00001000: 2074 6865 2064 6174 6166 7261 6d65 2061   the dataframe a
+00001010: 7320 6120 4475 636b 4442 2074 6162 6c65  s a DuckDB table
+00001020: 0a37 2e20 4578 6563 7574 6520 7468 6520  .7. Execute the 
+00001030: 5351 4c20 616e 6420 636f 6e76 6572 7420  SQL and convert 
+00001040: 746f 2061 2064 6174 6166 7261 6d65 0a0a  to a dataframe..
+00001050: 596f 7520 6d69 6768 7420 6e6f 7420 7761  You might not wa
+00001060: 6e74 2074 6f20 6368 6169 6e20 7468 6520  nt to chain the 
+00001070: 6f70 6572 6174 696f 6e73 206c 696b 6520  operations like 
+00001080: 7468 6973 2c20 616e 6420 7374 7269 6374  this, and strict
+00001090: 6c79 2073 7065 616b 696e 6720 6974 206d  ly speaking it m
+000010a0: 6967 6874 206e 6f74 2062 6520 7468 6520  ight not be the 
+000010b0: 6d6f 7374 2065 6666 6963 6965 6e74 2c20  most efficient, 
+000010c0: 0a67 6976 656e 2068 6f77 206d 7563 6820  .given how much 
+000010d0: 776f 726b 2068 6170 7065 6e73 2077 6974  work happens wit
+000010e0: 6869 6e20 7468 6f73 6520 6c69 6e65 7320  hin those lines 
+000010f0: 6f66 2063 6f64 652e 2054 6869 7320 6775  of code. This gu
+00001100: 6964 6520 7769 6c6c 2073 686f 7720 796f  ide will show yo
+00001110: 7520 7374 6570 2062 7920 7374 6570 0a68  u step by step.h
+00001120: 6f77 2074 6f20 6561 7369 6c79 2067 6574  ow to easily get
+00001130: 2053 4543 2066 696c 696e 6720 6461 7461   SEC filing data
+00001140: 2061 6e64 2074 6578 7420 696e 746f 2079   and text into y
+00001150: 6f75 7220 616e 616c 7974 6963 2077 6f72  our analytic wor
+00001160: 6b66 6c6f 7773 2e0a 0a0a 2323 2046 6561  kflows....## Fea
+00001170: 7475 7265 730a 0a2d 2044 6f77 6e6c 6f61  tures..- Downloa
+00001180: 6420 6c69 7374 696e 6773 206f 6620 4564  d listings of Ed
+00001190: 6761 7220 6669 6c69 6e67 2062 7920 7965  gar filing by ye
+000011a0: 6172 2c20 7175 6172 7465 7220 7369 6e63  ar, quarter sinc
+000011b0: 6520 3139 3934 0a2d 2053 656c 6563 7420  e 1994.- Select 
+000011c0: 616e 2069 6e64 6976 6964 7561 6c20 6669  an individual fi
+000011d0: 6c69 6e67 2061 6e64 2064 6f77 6e6c 6f61  ling and downloa
+000011e0: 6420 7468 6520 6874 6d6c 2c20 584d 4c20  d the html, XML 
+000011f0: 6f72 2063 6f6e 7465 6e74 206f 6620 616e  or content of an
+00001200: 7920 6174 7461 6368 6564 2066 696c 650a  y attached file.
+00001210: 2d20 5669 6577 2061 2066 696c 696e 6720  - View a filing 
+00001220: 5842 524c 2061 7320 6120 6461 7461 6672  XBRL as a datafr
+00001230: 616d 6520 616e 6420 7175 6572 7920 6974  ame and query it
+00001240: 2077 6974 6820 5351 4c0a 2d20 5365 6172   with SQL.- Sear
+00001250: 6368 2066 6f72 2063 6f6d 7061 6e79 2062  ch for company b
+00001260: 7920 7469 636b 6572 206f 7220 4349 4b0a  y ticker or CIK.
+00001270: 2d20 4765 7420 6120 636f 6d70 616e 7927  - Get a company'
+00001280: 7320 6669 6c69 6e67 7320 0a2d 2047 6574  s filings .- Get
+00001290: 2061 2064 6174 6173 6574 206f 6620 636f   a dataset of co
+000012a0: 6d70 616e 7927 7320 2a2a 6661 6374 732a  mpany's **facts*
+000012b0: 2a20 652e 672e 202a 2a43 6f6d 6d6f 6e53  * e.g. **CommonS
+000012c0: 6861 7265 734f 7574 7374 616e 6469 6e67  haresOutstanding
+000012d0: 2a2a 0a2d 2051 7565 7279 2061 2063 6f6d  **.- Query a com
+000012e0: 7061 6e79 2773 2066 6163 7473 2061 7320  pany's facts as 
+000012f0: 5351 4c20 7573 696e 6720 616e 2069 6e2d  SQL using an in-
+00001300: 6d65 6d6f 7279 202a 2a44 7563 6b44 422a  memory **DuckDB*
+00001310: 2a20 6461 7461 6261 7365 0a0a 2320 496e  * database..# In
+00001320: 7374 616c 6c61 7469 6f6e 0a0a 6060 6063  stallation..```c
+00001330: 6f6e 736f 6c65 0a70 6970 2069 6e73 7461  onsole.pip insta
+00001340: 6c6c 2065 6467 6172 746f 6f6c 730a 6060  ll edgartools.``
+00001350: 600a 0a23 2055 7361 6765 0a0a 0a23 2320  `..# Usage...## 
+00001360: 5365 7420 796f 7572 2045 6467 6172 2075  Set your Edgar u
+00001370: 7365 7220 6964 656e 7469 7479 0a0a 4265  ser identity..Be
+00001380: 666f 7265 2079 6f75 2063 616e 2061 6363  fore you can acc
+00001390: 6573 7320 7468 6520 5345 4320 4564 6761  ess the SEC Edga
+000013a0: 7220 4150 4920 796f 7520 6e65 6564 2074  r API you need t
+000013b0: 6f20 7365 7420 7468 6520 6964 656e 7469  o set the identi
+000013c0: 7479 2074 6861 7420 796f 7520 7769 6c6c  ty that you will
+000013d0: 2075 7365 2074 6f20 6163 6365 7373 2045   use to access E
+000013e0: 6467 6172 2e0a 5468 6973 2069 7320 7573  dgar..This is us
+000013f0: 7561 6c6c 7920 796f 7572 206e 616d 6520  ually your name 
+00001400: 616e 6420 656d 6169 6c2c 206f 7220 6120  and email, or a 
+00001410: 636f 6d70 616e 7920 6e61 6d65 2061 6e64  company name and
+00001420: 2065 6d61 696c 2e0a 6060 6062 6173 680a   email..```bash.
+00001430: 5361 6d70 6c65 2043 6f6d 7061 6e79 204e  Sample Company N
+00001440: 616d 6520 4164 6d69 6e43 6f6e 7461 6374  ame AdminContact
+00001450: 403c 7361 6d70 6c65 2063 6f6d 7061 6e79  @<sample company
+00001460: 2064 6f6d 6169 6e3e 2e63 6f6d 0a60 6060   domain>.com.```
+00001470: 0a0a 5468 6520 7573 6572 2069 6465 6e74  ..The user ident
+00001480: 6974 7920 6973 2073 656e 7420 696e 2074  ity is sent in t
+00001490: 6865 2055 7365 722d 4167 656e 7420 7374  he User-Agent st
+000014a0: 7269 6e67 2061 6e64 2074 6865 2045 6467  ring and the Edg
+000014b0: 6172 2041 5049 2077 696c 6c20 7265 6675  ar API will refu
+000014c0: 7365 2074 6f20 7265 7370 6f6e 6420 746f  se to respond to
+000014d0: 2079 6f75 7220 7265 7175 6573 7420 7769   your request wi
+000014e0: 7468 6f75 7420 6974 2e0a 0a45 6467 6172  thout it...Edgar
+000014f0: 546f 6f6c 7320 7769 6c6c 206c 6f6f 6b20  Tools will look 
+00001500: 666f 7220 616e 2065 6e76 6972 6f6e 6d65  for an environme
+00001510: 6e74 2076 6172 6961 626c 6520 6361 6c6c  nt variable call
+00001520: 6564 2060 4544 4741 525f 4944 454e 5449  ed `EDGAR_IDENTI
+00001530: 5459 6020 616e 6420 7573 6520 7468 6174  TY` and use that
+00001540: 2069 6e20 6561 6368 2072 6571 7565 7374   in each request
+00001550: 2e0a 536f 2c20 796f 7520 6e65 6564 2074  ..So, you need t
+00001560: 6f20 7365 7420 7468 6973 2065 6e76 6972  o set this envir
+00001570: 6f6e 6d65 6e74 2076 6172 6961 626c 6520  onment variable 
+00001580: 6265 666f 7265 2075 7369 6e67 2069 742e  before using it.
+00001590: 0a0a 2323 2320 5365 7474 696e 6720 4544  ..### Setting ED
+000015a0: 4741 525f 4944 454e 5449 5459 2069 6e20  GAR_IDENTITY in 
+000015b0: 4c69 6e75 782f 4d61 630a 6060 6062 6173  Linux/Mac.```bas
+000015c0: 680a 6578 706f 7274 2045 4447 4152 5f49  h.export EDGAR_I
+000015d0: 4445 4e54 4954 593d 224d 6963 6861 656c  DENTITY="Michael
+000015e0: 204d 6363 616c 6c75 6d20 6d63 616c 756d   Mccallum mcalum
+000015f0: 4067 6d61 696c 2e63 6f6d 220a 6060 600a  @gmail.com".```.
+00001600: 0a23 2323 2053 6574 7469 6e67 2045 4447  .### Setting EDG
+00001610: 4152 5f49 4445 4e54 4954 5920 696e 2057  AR_IDENTITY in W
+00001620: 696e 646f 7773 2050 6f77 6572 7368 656c  indows Powershel
+00001630: 6c0a 6060 6062 6173 680a 2024 456e 763a  l.```bash. $Env:
+00001640: 4544 4741 525f 4944 454e 5449 5459 3d22  EDGAR_IDENTITY="
+00001650: 4d69 6368 6165 6c20 4d63 6361 6c6c 756d  Michael Mccallum
+00001660: 206d 6361 6c75 6d40 676d 6169 6c2e 636f   mcalum@gmail.co
+00001670: 6d22 0a60 6060 0a41 6c74 6572 6e61 7469  m".```.Alternati
+00001680: 7665 6c79 2c20 796f 7520 6361 6e20 6361  vely, you can ca
+00001690: 6c6c 2060 7365 745f 6964 656e 7469 7479  ll `set_identity
+000016a0: 6020 7768 6963 6820 646f 6573 2074 6865  ` which does the
+000016b0: 2073 616d 6520 7468 696e 672e 0a0a 6060   same thing...``
+000016c0: 6070 7974 686f 6e0a 6672 6f6d 2065 6467  `python.from edg
+000016d0: 6172 2069 6d70 6f72 7420 7365 745f 6964  ar import set_id
+000016e0: 656e 7469 7479 0a73 6574 5f69 6465 6e74  entity.set_ident
+000016f0: 6974 7928 224d 6963 6861 656c 204d 6363  ity("Michael Mcc
+00001700: 616c 6c75 6d20 6d63 616c 756d 4067 6d61  allum mcalum@gma
+00001710: 696c 2e63 6f6d 2229 0a60 6060 0a46 6f72  il.com").```.For
+00001720: 206d 6f72 6520 6465 7461 696c 2073 6565   more detail see
+00001730: 2068 7474 7073 3a2f 2f77 7777 2e73 6563   https://www.sec
+00001740: 2e67 6f76 2f6f 732f 6163 6365 7373 696e  .gov/os/accessin
+00001750: 672d 6564 6761 722d 6461 7461 0a0a 0a23  g-edgar-data...#
+00001760: 2320 4765 7474 696e 6720 6669 6c69 6e67  # Getting filing
+00001770: 730a 546f 2067 6574 2073 7461 7274 6564  s.To get started
+00001780: 2069 6d70 6f72 7420 6672 6f6d 2065 6467   import from edg
+00001790: 6172 2061 6e64 2075 7365 2074 6865 2060  ar and use the `
+000017a0: 6765 745f 6669 6c69 6e67 7360 2066 756e  get_filings` fun
+000017b0: 6374 696f 6e2e 0a60 6060 7079 7468 6f6e  ction..```python
+000017c0: 0a66 726f 6d20 6564 6761 7220 696d 706f  .from edgar impo
+000017d0: 7274 202a 0a0a 6669 6c69 6e67 7320 3d20  rt *..filings = 
+000017e0: 6765 745f 6669 6c69 6e67 7328 290a 6060  get_filings().``
+000017f0: 600a 0a54 6869 7320 6765 7473 2074 6865  `..This gets the
+00001800: 206c 6973 7420 6f66 2066 696c 696e 6773   list of filings
+00001810: 2066 6f72 2074 6865 2063 7572 7265 6e74   for the current
+00001820: 2079 6561 7220 616e 6420 7175 6172 7465   year and quarte
+00001830: 7220 696e 746f 2061 2060 4669 6c69 6e67  r into a `Filing
+00001840: 7360 206f 626a 6563 742e 200a 0a21 5b47  s` object. ..![G
+00001850: 6574 2046 696c 696e 6773 5d28 6874 7470  et Filings](http
+00001860: 733a 2f2f 7261 772e 6769 7468 7562 7573  s://raw.githubus
+00001870: 6572 636f 6e74 656e 742e 636f 6d2f 6467  ercontent.com/dg
+00001880: 756e 6e69 6e67 2f65 6467 6172 746f 6f6c  unning/edgartool
+00001890: 732f 6d61 696e 2f69 6d61 6765 732f 6765  s/main/images/ge
+000018a0: 745f 6669 6c69 6e67 732e 6a70 6729 0a0a  t_filings.jpg)..
+000018b0: 4966 2079 6f75 206e 6565 6420 6120 6469  If you need a di
+000018c0: 6666 6572 656e 7420 6461 7465 2072 616e  fferent date ran
+000018d0: 6765 2079 6f75 2063 616e 2073 7065 6369  ge you can speci
+000018e0: 6679 2061 2079 6561 7220 6f72 2079 6561  fy a year or yea
+000018f0: 7273 2061 6e64 2061 2071 7561 7274 6572  rs and a quarter
+00001900: 206f 7220 7175 6172 7465 7273 2e0a 5468   or quarters..Th
+00001910: 6573 6520 6172 6520 7661 6c69 6420 7761  ese are valid wa
+00001920: 7973 2074 6f20 7370 6563 6966 7920 7468  ys to specify th
+00001930: 6520 6461 7465 2072 616e 6765 206f 7220  e date range or 
+00001940: 6669 6c74 6572 2062 7920 666f 726d 206f  filter by form o
+00001950: 7220 6279 2066 696c 696e 6720 6461 7465  r by filing date
+00001960: 2e0a 0a60 6060 7079 7468 6f6e 0a0a 2020  ...```python..  
+00001970: 2020 3e3e 3e20 6669 6c69 6e67 7320 3d20    >>> filings = 
+00001980: 6765 745f 6669 6c69 6e67 7328 3230 3231  get_filings(2021
+00001990: 2920 2320 4765 7420 6669 6c69 6e67 7320  ) # Get filings 
+000019a0: 666f 7220 3230 3231 0a0a 2020 2020 3e3e  for 2021..    >>
+000019b0: 3e20 6669 6c69 6e67 7320 3d20 6765 745f  > filings = get_
+000019c0: 6669 6c69 6e67 7328 3230 3231 2c20 3429  filings(2021, 4)
+000019d0: 2023 2047 6574 2066 696c 696e 6773 2066   # Get filings f
+000019e0: 6f72 2032 3032 3120 5134 0a0a 2020 2020  or 2021 Q4..    
+000019f0: 3e3e 3e20 6669 6c69 6e67 7320 3d20 6765  >>> filings = ge
+00001a00: 745f 6669 6c69 6e67 7328 3230 3231 2c20  t_filings(2021, 
+00001a10: 5b33 2c34 5d29 2023 2047 6574 2066 696c  [3,4]) # Get fil
+00001a20: 696e 6773 2066 6f72 2032 3032 3120 5133  ings for 2021 Q3
+00001a30: 2061 6e64 2051 340a 0a20 2020 203e 3e3e   and Q4..    >>>
+00001a40: 2066 696c 696e 6773 203d 2067 6574 5f66   filings = get_f
+00001a50: 696c 696e 6773 285b 3230 3230 2c20 3230  ilings([2020, 20
+00001a60: 3231 5d29 2023 2047 6574 2066 696c 696e  21]) # Get filin
+00001a70: 6773 2066 6f72 2032 3032 3020 616e 6420  gs for 2020 and 
+00001a80: 3230 3231 0a0a 2020 2020 3e3e 3e20 6669  2021..    >>> fi
+00001a90: 6c69 6e67 7320 3d20 6765 745f 6669 6c69  lings = get_fili
+00001aa0: 6e67 7328 5b32 3032 302c 2032 3032 315d  ngs([2020, 2021]
+00001ab0: 2c20 3429 2023 2047 6574 2066 696c 696e  , 4) # Get filin
+00001ac0: 6773 2066 6f72 2051 3420 6f66 2032 3032  gs for Q4 of 202
+00001ad0: 3020 616e 6420 3230 3231 0a0a 2020 2020  0 and 2021..    
+00001ae0: 3e3e 3e20 6669 6c69 6e67 7320 3d20 6765  >>> filings = ge
+00001af0: 745f 6669 6c69 6e67 7328 7261 6e67 6528  t_filings(range(
+00001b00: 3230 3130 2c20 3230 3231 2929 2023 2047  2010, 2021)) # G
+00001b10: 6574 2066 696c 696e 6773 2062 6574 7765  et filings betwe
+00001b20: 656e 2032 3031 3020 616e 6420 3230 3231  en 2010 and 2021
+00001b30: 202d 2064 6f65 7320 6e6f 7420 696e 636c   - does not incl
+00001b40: 7564 6520 3230 3231 0a0a 2020 2020 3e3e  ude 2021..    >>
+00001b50: 3e20 6669 6c69 6e67 7320 3d20 6765 745f  > filings = get_
+00001b60: 6669 6c69 6e67 7328 3230 3231 2c20 342c  filings(2021, 4,
+00001b70: 2066 6f72 6d3d 2244 2229 2023 2047 6574   form="D") # Get
+00001b80: 2066 696c 696e 6773 2066 6f72 2032 3032   filings for 202
+00001b90: 3120 5134 2066 6f72 2066 6f72 6d20 440a  1 Q4 for form D.
+00001ba0: 0a20 2020 203e 3e3e 2066 696c 696e 6773  .    >>> filings
+00001bb0: 203d 2067 6574 5f66 696c 696e 6773 2832   = get_filings(2
+00001bc0: 3032 312c 2034 2c20 6669 6c69 6e67 5f64  021, 4, filing_d
+00001bd0: 6174 653d 2232 3032 312d 3130 2d30 3122  ate="2021-10-01"
+00001be0: 2920 2320 4765 7420 6669 6c69 6e67 7320  ) # Get filings 
+00001bf0: 666f 7220 3230 3231 2051 3420 6f6e 2022  for 2021 Q4 on "
+00001c00: 3230 3231 2d31 302d 3031 220a 0a20 2020  2021-10-01"..   
+00001c10: 203e 3e3e 2066 696c 696e 6773 203d 2067   >>> filings = g
+00001c20: 6574 5f66 696c 696e 6773 2832 3032 312c  et_filings(2021,
+00001c30: 2034 2c20 6669 6c69 6e67 5f64 6174 653d   4, filing_date=
+00001c40: 2232 3032 312d 3130 2d30 313a 3230 3231  "2021-10-01:2021
+00001c50: 2d31 302d 3130 2229 2023 2047 6574 2066  -10-10") # Get f
+00001c60: 696c 696e 6773 2066 6f72 2032 3032 3120  ilings for 2021 
+00001c70: 5134 2062 6574 7765 656e 0a20 2020 2020  Q4 between.     
+00001c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001cc0: 2020 2020 2020 2023 2022 3230 3231 2d31         # "2021-1
+00001cd0: 302d 3031 2220 616e 6420 2232 3032 312d  0-01" and "2021-
+00001ce0: 3130 2d31 3022 0a60 6060 0a0a 2323 2320  10-10".```..### 
+00001cf0: 436f 6e76 6572 7420 7468 6520 6669 6c69  Convert the fili
+00001d00: 6e67 7320 746f 2061 2070 616e 6461 7320  ngs to a pandas 
+00001d10: 6461 7461 6672 616d 650a 0a54 6865 2066  dataframe..The f
+00001d20: 696c 696e 6773 2064 6174 6120 6973 2073  ilings data is s
+00001d30: 746f 7265 6420 696e 2074 6865 2060 4669  tored in the `Fi
+00001d40: 6c69 6e67 7360 2063 6c61 7373 2061 7320  lings` class as 
+00001d50: 6120 6070 7961 7272 6f77 2e54 6162 6c65  a `pyarrow.Table
+00001d60: 602e 2059 6f75 2063 616e 2067 6574 2074  `. You can get t
+00001d70: 6865 2064 6174 6120 6173 2061 2070 616e  he data as a pan
+00001d80: 6461 7320 6461 7461 6672 616d 6520 7573  das dataframe us
+00001d90: 696e 670a 6074 6f5f 7061 6e64 6173 600a  ing.`to_pandas`.
+00001da0: 6060 6070 7974 686f 6e0a 6466 203d 2066  ```python.df = f
+00001db0: 696c 696e 6773 2e74 6f5f 7061 6e64 6173  ilings.to_pandas
+00001dc0: 2829 0a60 6060 0a0a 0a23 2320 4e61 7669  ().```...## Navi
+00001dd0: 6761 7469 6e67 2066 696c 696e 6773 0a0a  gating filings..
+00001de0: 5468 6520 4669 6c69 6e67 7320 6f62 6a65  The Filings obje
+00001df0: 6374 2061 6c6c 6f77 7320 796f 7520 746f  ct allows you to
+00001e00: 206e 6176 6967 6174 6520 7468 726f 7567   navigate throug
+00001e10: 6820 6669 6c69 6e67 7320 7573 696e 6720  h filings using 
+00001e20: 6066 696c 696e 6773 2e6e 6578 7428 2960  `filings.next()`
+00001e30: 2061 6e64 2060 6669 6c69 6e67 732e 7072   and `filings.pr
+00001e40: 6576 2829 602e 200a 5468 6973 2073 686f  ev()`. .This sho
+00001e50: 7773 2079 6f75 2070 6167 6573 206f 6620  ws you pages of 
+00001e60: 7468 6520 6461 7461 202d 2074 6865 2070  the data - the p
+00001e70: 6167 6520 7369 7a65 2069 7320 6162 6f75  age size is abou
+00001e80: 7420 3530 2e20 0a0a 6060 6070 7974 686f  t 50. ..```pytho
+00001e90: 6e0a 2320 546f 2073 6565 2074 6865 206e  n.# To see the n
+00001ea0: 6578 7420 7061 6765 206f 6620 6461 7461  ext page of data
+00001eb0: 0a66 696c 696e 6773 2e6e 6578 7428 290a  .filings.next().
+00001ec0: 0a23 2054 6f20 7365 6520 7468 6520 7072  .# To see the pr
+00001ed0: 6576 696f 7573 2070 6167 650a 6669 6c69  evious page.fili
+00001ee0: 6e67 732e 7072 6576 2829 0a0a 2320 546f  ngs.prev()..# To
+00001ef0: 2073 6565 2074 6865 2063 7572 7265 6e74   see the current
+00001f00: 2070 6167 650a 6669 6c69 6e67 732e 6375   page.filings.cu
+00001f10: 7272 656e 7428 290a 6060 600a 0a21 5b47  rrent().```..![G
+00001f20: 6574 206e 6578 7420 6669 6c69 6e67 735d  et next filings]
+00001f30: 2868 7474 7073 3a2f 2f72 6177 2e67 6974  (https://raw.git
+00001f40: 6875 6275 7365 7263 6f6e 7465 6e74 2e63  hubusercontent.c
+00001f50: 6f6d 2f64 6775 6e6e 696e 672f 6564 6761  om/dgunning/edga
+00001f60: 7274 6f6f 6c73 2f6d 6169 6e2f 696d 6167  rtools/main/imag
+00001f70: 6573 2f66 696c 696e 6773 5f6e 6578 742e  es/filings_next.
+00001f80: 6a70 6729 0a0a 2323 2047 6574 7469 6e67  jpg)..## Getting
+00001f90: 2074 6865 206c 6174 6573 7420 6669 6c69   the latest fili
+00001fa0: 6e67 730a 0a59 6f75 2063 616e 2067 6574  ngs..You can get
+00001fb0: 2074 6865 206c 6174 6573 7420 2a2a 6e2a   the latest **n*
+00001fc0: 2a20 6669 6c69 6e67 7320 6279 2066 696c  * filings by fil
+00001fd0: 696e 675f 6461 7465 2066 726f 6d20 6120  ing_date from a 
+00001fe0: 6669 6c69 6e67 7320 7573 696e 6720 6066  filings using `f
+00001ff0: 696c 696e 6773 2e6c 6174 6573 7428 2960  ilings.latest()`
+00002000: 2e0a 0a49 6620 796f 7520 7072 6f76 6964  ...If you provid
+00002010: 6520 7468 6520 7061 7261 6d65 7465 7220  e the parameter 
+00002020: 606e 6020 6974 2077 696c 6c20 7265 7475  `n` it will retu
+00002030: 726e 2074 6865 206c 6174 6573 7420 606e  rn the latest `n
+00002040: 6020 6669 6c69 6e67 732e 0a0a 6060 6070  ` filings...```p
+00002050: 7974 686f 6e0a 6669 6c69 6e67 203d 2066  ython.filing = f
+00002060: 696c 696e 6773 2e6c 6174 6573 7428 6e3d  ilings.latest(n=
+00002070: 3529 0a66 696c 696e 670a 6060 600a 215b  5).filing.```.![
+00002080: 4c61 7465 7374 2066 696c 696e 6773 5d28  Latest filings](
+00002090: 6874 7470 733a 2f2f 7261 772e 6769 7468  https://raw.gith
+000020a0: 7562 7573 6572 636f 6e74 656e 742e 636f  ubusercontent.co
+000020b0: 6d2f 6467 756e 6e69 6e67 2f65 6467 6172  m/dgunning/edgar
+000020c0: 746f 6f6c 732f 6d61 696e 2f69 6d61 6765  tools/main/image
+000020d0: 732f 6c61 7465 7374 5f66 696c 696e 6773  s/latest_filings
+000020e0: 2e6a 7067 290a 0a0a 4966 2079 6f75 206f  .jpg)...If you o
+000020f0: 6d69 7420 7468 6973 2070 6172 616d 6574  mit this paramet
+00002100: 6572 2c20 6f72 2073 6574 2060 6e3d 3160  er, or set `n=1`
+00002110: 2069 7420 7769 6c6c 2072 6574 7572 6e20   it will return 
+00002120: 6120 7369 6e67 6c65 2060 4669 6c69 6e67  a single `Filing
+00002130: 7320 6f62 6a65 6374 2e0a 0a60 6060 7079  s object...```py
+00002140: 7468 6f6e 0a66 696c 696e 6720 3d20 6669  thon.filing = fi
+00002150: 6c69 6e67 732e 6c61 7465 7374 2829 0a66  lings.latest().f
+00002160: 696c 696e 670a 6060 600a 215b 4c61 7465  iling.```.![Late
+00002170: 7374 2066 696c 696e 675d 2868 7474 7073  st filing](https
+00002180: 3a2f 2f72 6177 2e67 6974 6875 6275 7365  ://raw.githubuse
+00002190: 7263 6f6e 7465 6e74 2e63 6f6d 2f64 6775  rcontent.com/dgu
+000021a0: 6e6e 696e 672f 6564 6761 7274 6f6f 6c73  nning/edgartools
+000021b0: 2f6d 6169 6e2f 696d 6167 6573 2f6c 6174  /main/images/lat
+000021c0: 6573 745f 6669 6c69 6e67 2e6a 7067 290a  est_filing.jpg).
+000021d0: 0a0a 2323 2046 696c 7465 7269 6e67 2066  ..## Filtering f
+000021e0: 696c 696e 6773 0a0a 596f 7520 6361 6e20  ilings..You can 
+000021f0: 6669 6c74 6572 2074 6865 2066 696c 696e  filter the filin
+00002200: 6773 206f 626a 6563 7420 7573 696e 6720  gs object using 
+00002210: 7465 2060 6669 6c74 6572 2829 6020 6675  te `filter()` fu
+00002220: 6e63 7469 6f6e 2e20 5468 6973 2061 6c6c  nction. This all
+00002230: 6f77 7320 796f 7520 746f 2066 696c 7465  ows you to filte
+00002240: 720a 6279 2066 696c 696e 6720 6461 7465  r.by filing date
+00002250: 2c20 6f72 2062 7920 666f 726d 2e0a 0a23  , or by form...#
+00002260: 2323 2046 696c 7465 7269 6e67 2066 696c  ## Filtering fil
+00002270: 696e 6773 2062 7920 6461 7465 0a0a 546f  ings by date..To
+00002280: 2066 696c 7465 7220 6279 2066 696c 696e   filter by filin
+00002290: 6720 6461 7465 2073 7065 6369 6679 2074  g date specify t
+000022a0: 6865 2066 696c 696e 6720 6461 7465 2069  he filing date i
+000022b0: 6e20 2a2a 5959 5959 2d4d 4d2d 4444 2a2a  n **YYYY-MM-DD**
+000022c0: 2066 6f72 6d61 7420 652e 672e 202a 2a32   format e.g. **2
+000022d0: 3032 322d 3031 2d32 342a 2a0a 284e 6f74  022-01-24**.(Not
+000022e0: 6520 7468 6520 7061 7261 6d65 7465 7273  e the parameters
+000022f0: 2060 6461 7465 6020 616e 6420 6066 696c   `date` and `fil
+00002300: 696e 675f 6461 7465 6020 6172 6520 6571  ing_date` are eq
+00002310: 7569 7661 6c65 6e74 2061 6c69 6173 6573  uivalent aliases
+00002320: 2066 6f72 2065 6163 6820 6f74 6865 7229   for each other)
+00002330: 0a60 6060 7079 7468 6f6e 0a66 696c 696e  .```python.filin
+00002340: 6773 2e66 696c 7465 7228 6461 7465 3d22  gs.filter(date="
+00002350: 3230 3231 2d30 312d 3234 2229 2023 206f  2021-01-24") # o
+00002360: 7220 6669 6c69 6e67 732e 6669 6c74 6572  r filings.filter
+00002370: 2866 696c 696e 675f 6461 7465 3d22 3230  (filing_date="20
+00002380: 3231 2d30 312d 3234 2229 0a60 6060 0a59  21-01-24").```.Y
+00002390: 6f75 2063 616e 2073 7065 6369 6679 2061  ou can specify a
+000023a0: 2066 696c 696e 6720 6461 7465 2072 616e   filing date ran
+000023b0: 6765 2075 7369 6e67 2074 6865 2063 6f6c  ge using the col
+000023c0: 6f6e 0a0a 6060 6070 7974 686f 6e0a 6669  on..```python.fi
+000023d0: 6c69 6e67 732e 6669 6c74 6572 2864 6174  lings.filter(dat
+000023e0: 653d 2232 3032 312d 3031 2d31 323a 3230  e="2021-01-12:20
+000023f0: 3231 2d30 322d 3238 2229 200a 6060 600a  21-02-28") .```.
+00002400: 546f 2066 696c 7465 7220 6279 2064 6174  To filter by dat
+00002410: 6573 2062 6566 6f72 6520 6120 7370 6563  es before a spec
+00002420: 6966 6965 6420 6461 7465 2075 7365 2060  ified date use `
+00002430: 3a59 5959 592d 4d4d 2d44 4427 0a0a 6060  :YYYY-MM-DD'..``
+00002440: 6070 7974 686f 6e0a 6669 6c69 6e67 732e  `python.filings.
+00002450: 6669 6c74 6572 2864 6174 653d 223a 3230  filter(date=":20
+00002460: 3231 2d30 322d 3238 2229 200a 6060 600a  21-02-28") .```.
+00002470: 0a54 6f20 6669 6c74 6572 2062 7920 6461  .To filter by da
+00002480: 7465 7320 6166 7465 7220 6120 7370 6563  tes after a spec
+00002490: 6966 6965 6420 6461 7465 2075 7365 2060  ified date use `
+000024a0: 5959 5959 2d4d 4d2d 4444 3a27 0a0a 6060  YYYY-MM-DD:'..``
+000024b0: 6070 7974 686f 6e0a 6669 6c69 6e67 732e  `python.filings.
+000024c0: 6669 6c74 6572 2864 6174 653d 2232 3032  filter(date="202
+000024d0: 312d 3032 2d32 383a 2229 200a 6060 600a  1-02-28:") .```.
+000024e0: 0a23 2323 2046 696c 7465 7269 6e67 2066  .### Filtering f
+000024f0: 696c 696e 6773 2062 7920 666f 726d 0a0a  ilings by form..
+00002500: 596f 7520 6361 6e20 6669 6c74 6572 2066  You can filter f
+00002510: 696c 696e 6773 2062 7920 666f 726d 2075  ilings by form u
+00002520: 7369 6e67 2074 6865 2060 666f 726d 6020  sing the `form` 
+00002530: 7061 7261 6d65 7465 722e 200a 0a60 6060  parameter. ..```
+00002540: 7079 7468 6f6e 0a66 696c 696e 6773 2e66  python.filings.f
+00002550: 696c 7465 7228 666f 726d 3d22 3130 2d4b  ilter(form="10-K
+00002560: 2229 200a 6060 600a 0a54 6f20 6669 6c74  ") .```..To filt
+00002570: 6572 2062 7920 666f 726d 2065 2e67 2e20  er by form e.g. 
+00002580: 2a2a 3130 2d4b 2a2a 2061 6e64 2069 6e63  **10-K** and inc
+00002590: 6c75 6465 2066 6f72 6d20 616d 656e 646d  lude form amendm
+000025a0: 656e 7473 2075 7365 2060 616d 656e 646d  ents use `amendm
+000025b0: 656e 7473 203d 2054 7275 6560 2e20 0a0a  ents = True`. ..
+000025c0: 6060 6070 7974 686f 6e0a 6669 6c69 6e67  ```python.filing
+000025d0: 732e 6669 6c74 6572 2866 6f72 6d3d 2231  s.filter(form="1
+000025e0: 302d 4b22 2c20 616d 656e 646d 656e 7473  0-K", amendments
+000025f0: 3d54 7275 6529 200a 6060 600a 215b 4669  =True) .```.![Fi
+00002600: 6c74 6572 2077 6974 6820 616d 656e 646d  lter with amendm
+00002610: 656e 7473 5d28 6874 7470 733a 2f2f 7261  ents](https://ra
+00002620: 772e 6769 7468 7562 7573 6572 636f 6e74  w.githubusercont
+00002630: 656e 742e 636f 6d2f 6467 756e 6e69 6e67  ent.com/dgunning
+00002640: 2f65 6467 6172 746f 6f6c 732f 6d61 696e  /edgartools/main
+00002650: 2f69 6d61 6765 732f 6669 6c74 6572 5f61  /images/filter_a
+00002660: 6d65 6e64 6d65 6e74 732e 6a70 6729 0a0a  mendments.jpg)..
+00002670: 2323 2047 6574 7469 6e67 2061 2073 696e  ## Getting a sin
+00002680: 676c 6520 6669 6c69 6e67 0a0a 596f 7520  gle filing..You 
+00002690: 6361 6e20 6765 7420 6120 7369 6e67 6c65  can get a single
+000026a0: 2066 696c 696e 6720 6672 6f6d 2074 6865   filing from the
+000026b0: 2066 696c 696e 6773 2075 7369 6e67 2074   filings using t
+000026c0: 6865 2062 7261 636b 6574 206f 7065 7261  he bracket opera
+000026d0: 746f 7220 605b 5d60 2c20 0a73 7065 6369  tor `[]`, .speci
+000026e0: 6679 696e 6720 7468 6520 696e 6465 7820  fying the index 
+000026f0: 6f66 2074 6865 2066 696c 696e 672e 2054  of the filing. T
+00002700: 6865 2069 6e64 6578 2069 7320 7468 6520  he index is the 
+00002710: 7661 6c75 6520 6469 7370 6c61 7965 6420  value displayed 
+00002720: 696e 2074 6865 206c 6566 746d 6f73 740a  in the leftmost.
+00002730: 706f 7369 7469 6f6e 2069 6e20 7468 6520  position in the 
+00002740: 6669 6c69 6e67 7320 7461 626c 652e 2046  filings table. F
+00002750: 6f72 2065 7861 6d70 6c65 2c20 746f 2067  or example, to g
+00002760: 6574 2074 6865 202a 2a31 302d 512a 2a20  et the **10-Q** 
+00002770: 666f 7220 2a2a 436f 7374 636f 2a2a 2069  for **Costco** i
+00002780: 6e20 7468 6520 7461 626c 6520 6162 6f76  n the table abov
+00002790: 650a 7573 6520 6066 696c 696e 6773 5b33  e.use `filings[3
+000027a0: 5d60 0a0a 6060 6070 7974 686f 6e0a 6669  ]`..```python.fi
+000027b0: 6c69 6e67 203d 2066 696c 696e 6773 5b33  ling = filings[3
+000027c0: 5d0a 6060 600a 0a21 5b43 6f73 7463 6f20  ].```..![Costco 
+000027d0: 3130 5120 6669 6c69 6e67 5d28 6874 7470  10Q filing](http
+000027e0: 733a 2f2f 7261 772e 6769 7468 7562 7573  s://raw.githubus
+000027f0: 6572 636f 6e74 656e 742e 636f 6d2f 6467  ercontent.com/dg
+00002800: 756e 6e69 6e67 2f65 6467 6172 746f 6f6c  unning/edgartool
+00002810: 732f 6d61 696e 2f69 6d61 6765 732f 636f  s/main/images/co
+00002820: 7374 636f 5f31 3051 2e6a 7067 290a 0a23  stco_10Q.jpg)..#
+00002830: 2323 2056 6965 7720 7468 6520 6669 6c69  ## View the fili
+00002840: 6e67 2068 6f6d 6570 6167 650a 596f 7520  ng homepage.You 
+00002850: 6361 6e20 7669 6577 2074 6865 2066 696c  can view the fil
+00002860: 696e 6720 686f 6d65 7061 6765 2069 6e20  ing homepage in 
+00002870: 7468 6520 7465 726d 696e 616c 2075 7369  the terminal usi
+00002880: 6e67 2060 6669 6c69 6e67 2e68 6f6d 6570  ng `filing.homep
+00002890: 6167 6560 0a0a 5468 6973 2067 6976 6573  age`..This gives
+000028a0: 2079 6f75 2061 6363 6573 7320 746f 2074   you access to t
+000028b0: 6865 2060 4669 6c69 6e67 486f 6d65 7061  he `FilingHomepa
+000028c0: 6765 6020 636c 6173 7320 7468 6174 2079  ge` class that y
+000028d0: 6f75 2063 616e 2075 7365 2074 6f20 6c69  ou can use to li
+000028e0: 7374 2061 6c6c 2074 6865 2064 6f63 756d  st all the docum
+000028f0: 656e 7473 0a61 6e64 2064 6174 6166 696c  ents.and datafil
+00002900: 6573 206f 6e20 7468 6520 6669 6c69 6e67  es on the filing
+00002910: 2e0a 0a60 6060 7079 7468 6f6e 0a66 696c  ...```python.fil
+00002920: 696e 672e 686f 6d65 7061 6765 0a60 6060  ing.homepage.```
+00002930: 0a21 5b46 696c 696e 6720 686f 6d61 7061  .![Filing homapa
+00002940: 6765 5d28 6874 7470 733a 2f2f 7261 772e  ge](https://raw.
+00002950: 6769 7468 7562 7573 6572 636f 6e74 656e  githubuserconten
+00002960: 742e 636f 6d2f 6467 756e 6e69 6e67 2f65  t.com/dgunning/e
+00002970: 6467 6172 746f 6f6c 732f 6d61 696e 2f69  dgartools/main/i
+00002980: 6d61 6765 732f 6669 6c69 6e67 5f68 6f6d  mages/filing_hom
+00002990: 6570 6167 652e 6a70 6729 0a0a 2323 2320  epage.jpg)..### 
+000029a0: 4f70 656e 2061 2066 696c 696e 670a 0a59  Open a filing..Y
+000029b0: 6f75 2063 616e 206f 7065 6e20 7468 6520  ou can open the 
+000029c0: 6669 6c69 6e67 2069 6e20 796f 7572 2062  filing in your b
+000029d0: 726f 7773 6572 2075 7369 6e67 2060 6669  rowser using `fi
+000029e0: 6c69 6e67 2e6f 7065 6e28 2960 2e20 5468  ling.open()`. Th
+000029f0: 6973 2077 696c 6c20 776f 726b 206f 6e20  is will work on 
+00002a00: 656e 7669 726f 6e6d 656e 7473 2077 6974  environments wit
+00002a10: 6820 6163 6365 7373 2074 6f20 7468 6520  h access to the 
+00002a20: 6272 6f77 7365 722c 200a 7769 6c6c 2070  browser, .will p
+00002a30: 726f 6261 626c 7920 6e6f 7420 776f 726b  robably not work
+00002a40: 206f 6e20 6120 7265 6d6f 7465 2073 6572   on a remote ser
+00002a50: 7665 722e 0a60 6060 7079 7468 6f6e 0a66  ver..```python.f
+00002a60: 696c 696e 672e 6f70 656e 2829 0a60 6060  iling.open().```
+00002a70: 0a0a 2323 2320 4f70 656e 2074 6865 2046  ..### Open the F
+00002a80: 696c 696e 6720 486f 6d65 7061 6765 0a59  iling Homepage.Y
+00002a90: 6f75 2063 616e 206f 7065 6e20 7468 6520  ou can open the 
+00002aa0: 6669 6c69 6e67 2068 6f6d 6570 6167 6520  filing homepage 
+00002ab0: 696e 2074 6865 2062 726f 7773 6572 2075  in the browser u
+00002ac0: 7369 6e67 2060 6669 6c69 6e67 2e68 6f6d  sing `filing.hom
+00002ad0: 6570 6167 652e 6f70 656e 2829 602e 0a60  epage.open()`..`
+00002ae0: 6060 7079 7468 6f6e 0a66 696c 696e 672e  ``python.filing.
+00002af0: 686f 6d65 7061 6765 2e6f 7065 6e28 290a  homepage.open().
+00002b00: 6060 600a 0a23 2323 2057 6f72 6b69 6e67  ```..### Working
+00002b10: 2077 6974 6820 5842 524c 2066 696c 696e   with XBRL filin
+00002b20: 6773 0a0a 536f 6d65 2066 696c 696e 6773  gs..Some filings
+00002b30: 2061 7265 2069 6e20 2a2a 5842 524c 2028   are in **XBRL (
+00002b40: 6558 7465 6e73 6962 6c65 2042 7573 696e  eXtensible Busin
+00002b50: 6573 7320 4d61 726b 7570 204c 616e 6775  ess Markup Langu
+00002b60: 6167 6529 2a2a 2066 6f72 6d61 742e 200a  age)** format. .
+00002b70: 5468 6573 6520 6172 6520 6d61 696e 6c79  These are mainly
+00002b80: 2074 6865 206e 6577 6572 2066 696c 696e   the newer filin
+00002b90: 6773 2c20 6173 2074 6865 2053 4543 2068  gs, as the SEC h
+00002ba0: 6173 2073 7461 7274 6564 2072 6571 7569  as started requi
+00002bb0: 7269 6e67 2074 6869 7320 666f 7220 6e65  ring this for ne
+00002bc0: 7765 7220 6669 6c69 6e67 732e 0a0a 4966  wer filings...If
+00002bd0: 2061 2066 696c 696e 6720 6973 2069 6e20   a filing is in 
+00002be0: 5842 524c 2066 6f72 6d61 7420 7468 656e  XBRL format then
+00002bf0: 2069 7420 6f70 656e 7320 7570 2061 206c   it opens up a l
+00002c00: 6f74 206d 6f72 6520 7761 7973 2074 6f20  ot more ways to 
+00002c10: 6765 7420 7374 7275 6374 7572 6564 2064  get structured d
+00002c20: 6174 6120 6162 6f75 7420 7468 6174 2073  ata about that s
+00002c30: 7065 6369 6669 6320 6669 6c69 6e67 2061  pecific filing a
+00002c40: 6e64 2061 6c73 6f20 0a61 626f 7574 2074  nd also .about t
+00002c50: 6865 2063 6f6d 7061 6e79 2072 6566 6572  he company refer
+00002c60: 7265 6420 746f 2069 6e20 7468 6174 2066  red to in that f
+00002c70: 696c 696e 672e 0a0a 5468 6520 6046 696c  iling...The `Fil
+00002c80: 696e 6760 2063 6c61 7373 2068 6173 2061  ing` class has a
+00002c90: 6e20 6078 6272 6c60 2066 756e 6374 696f  n `xbrl` functio
+00002ca0: 6e20 7468 6174 2077 696c 6c20 646f 776e  n that will down
+00002cb0: 6c6f 6164 2c20 7061 7273 6520 616e 6420  load, parse and 
+00002cc0: 7374 7275 6374 7572 6520 7468 6520 6669  structure the fi
+00002cd0: 6c69 6e67 2773 2058 4252 4c20 646f 6375  ling's XBRL docu
+00002ce0: 6d65 6e74 2069 6620 6f6e 6520 6578 6973  ment if one exis
+00002cf0: 7473 2e0a 4966 2069 7420 646f 6573 206e  ts..If it does n
+00002d00: 6f74 2065 7869 7374 2c20 7468 656e 2060  ot exist, then `
+00002d10: 6669 6c69 6e67 2e78 6272 6c28 2960 2077  filing.xbrl()` w
+00002d20: 696c 6c20 7265 7475 726e 2060 4e6f 6e65  ill return `None
+00002d30: 602e 0a0a 5468 6520 6675 6e63 7469 6f6e  `...The function
+00002d40: 2060 6669 6c69 6e67 2e78 6272 6c28 2960   `filing.xbrl()`
+00002d50: 2072 6574 7572 6e73 2061 2060 4669 6c69   returns a `Fili
+00002d60: 6e67 5862 726c 6020 696e 7374 616e 6365  ngXbrl` instance
+00002d70: 2c20 7768 6963 6820 7772 6170 7320 7468  , which wraps th
+00002d80: 6520 6461 7461 2c20 616e 6420 7072 6f76  e data, and prov
+00002d90: 6964 6573 2063 6f6e 7665 6e69 656e 740a  ides convenient.
+00002da0: 7761 7973 206f 6620 776f 726b 696e 6720  ways of working 
+00002db0: 7769 7468 2074 6865 2078 6272 6c20 6461  with the xbrl da
+00002dc0: 7461 2e0a 0a0a 6060 6070 7974 686f 6e0a  ta....```python.
+00002dd0: 6669 6c69 6e67 5f78 6272 6c20 3d20 6669  filing_xbrl = fi
+00002de0: 6c69 6e67 2e78 6272 6c28 290a 6060 600a  ling.xbrl().```.
+00002df0: 0a21 5b46 696c 696e 6720 686f 6d61 7061  .![Filing homapa
+00002e00: 6765 5d28 6874 7470 733a 2f2f 7261 772e  ge](https://raw.
+00002e10: 6769 7468 7562 7573 6572 636f 6e74 656e  githubuserconten
+00002e20: 742e 636f 6d2f 6467 756e 6e69 6e67 2f65  t.com/dgunning/e
+00002e30: 6467 6172 746f 6f6c 732f 6d61 696e 2f69  dgartools/main/i
+00002e40: 6d61 6765 732f 3130 515f 7862 726c 2e6a  mages/10Q_xbrl.j
+00002e50: 7067 290a 0a0a 2323 2323 2055 7365 2044  pg)...#### Use D
+00002e60: 7563 6b44 4220 746f 2071 7565 7279 2074  uckDB to query t
+00002e70: 6865 2066 696c 696e 6773 0a0a 4120 636f  he filings..A co
+00002e80: 6e76 6569 656e 7420 7761 7920 746f 2071  nveient way to q
+00002e90: 7565 7279 2074 6865 2066 696c 696e 6773  uery the filings
+00002ea0: 2064 6174 6120 6973 2074 6f20 7573 6520   data is to use 
+00002eb0: 2a2a 4475 636b 4442 2a2a 2e20 4966 2079  **DuckDB**. If y
+00002ec0: 6f75 2063 616c 6c20 7468 6520 6074 6f5f  ou call the `to_
+00002ed0: 6475 636b 6462 6020 6675 6e63 7469 6f6e  duckdb` function
+00002ee0: 2c20 796f 7520 6765 7420 616e 2069 6e2d  , you get an in-
+00002ef0: 6d65 6d6f 7279 0a44 7563 6b44 4220 6461  memory.DuckDB da
+00002f00: 7461 6261 7365 2069 6e73 7461 6e63 652c  tabase instance,
+00002f10: 2077 6974 6820 7468 6520 6669 6c69 6e67   with the filing
+00002f20: 7320 7265 6769 7374 6572 6564 2061 7320  s registered as 
+00002f30: 6120 7461 626c 6520 6361 6c6c 6564 2060  a table called `
+00002f40: 6669 6c69 6e67 7360 2e0a 5468 656e 2079  filings`..Then y
+00002f50: 6f75 2063 616e 2077 6f72 6b20 6469 7265  ou can work dire
+00002f60: 6374 7920 7769 7468 2074 6865 2044 7563  cty with the Duc
+00002f70: 6b44 4220 6461 7461 6261 7365 2c20 616e  kDB database, an
+00002f80: 6420 7275 6e20 5351 4c20 6167 6169 6e73  d run SQL agains
+00002f90: 7420 7468 6520 6669 6c69 6e67 7320 6461  t the filings da
+00002fa0: 7461 2e0a 0a49 6e20 7468 6973 2065 7861  ta...In this exa
+00002fb0: 6d70 6c65 2c20 7765 2066 696c 7465 7220  mple, we filter 
+00002fc0: 6669 6c69 6e67 7320 666f 7220 2a2a 532d  filings for **S-
+00002fd0: 312a 2a20 666f 726d 2074 7970 6573 2e0a  1** form types..
+00002fe0: 0a60 6060 7079 7468 6f6e 0a64 6220 3d20  .```python.db = 
+00002ff0: 6669 6c69 6e67 732e 746f 5f64 7563 6b64  filings.to_duckd
+00003000: 6228 290a 2320 6120 6475 636b 6462 2e44  b().# a duckdb.D
+00003010: 7563 6b44 4250 7943 6f6e 6e65 6374 696f  uckDBPyConnectio
+00003020: 6e0a 0a23 2051 7565 7279 2074 6865 2066  n..# Query the f
+00003030: 696c 696e 6773 2066 6f72 2053 2d31 2066  ilings for S-1 f
+00003040: 696c 696e 6773 2061 6e64 2072 6574 7572  ilings and retur
+00003050: 6e20 6120 6461 7461 6672 616d 650a 6462  n a dataframe.db
+00003060: 2e65 7865 6375 7465 2822 2222 0a73 656c  .execute(""".sel
+00003070: 6563 7420 2a20 6672 6f6d 2066 696c 696e  ect * from filin
+00003080: 6773 2077 6865 7265 2046 6f72 6d20 3d3d  gs where Form ==
+00003090: 2027 532d 3127 0a22 2222 292e 6466 2829   'S-1'.""").df()
+000030a0: 0a60 6060 0a0a 0a23 2320 5573 696e 6720  .```...## Using 
+000030b0: 7468 6520 436f 6d70 616e 7920 4150 490a  the Company API.
+000030c0: 0a57 6974 6820 7468 6520 636f 6d70 616e  .With the compan
+000030d0: 7920 4150 4920 796f 7520 6669 6e64 2061  y API you find a
+000030e0: 2063 6f6d 7061 6e79 2075 7369 6e67 2074   company using t
+000030f0: 6865 202a 2a63 696b 2a2a 206f 7220 2a2a  he **cik** or **
+00003100: 7469 636b 6572 2a2a 2e20 0a46 726f 6d20  ticker**. .From 
+00003110: 7468 6520 636f 6d70 616e 7920 796f 7520  the company you 
+00003120: 6361 6e20 6163 6365 7373 2061 6c6c 2074  can access all t
+00003130: 6865 6972 2068 6973 746f 7269 6361 6c20  heir historical 
+00003140: 2a2a 6669 6c69 6e67 732a 2a2c 0a61 6e64  **filings**,.and
+00003150: 2061 2064 6174 6173 6574 206f 6620 7468   a dataset of th
+00003160: 6520 636f 6d70 616e 7920 2a2a 6661 6374  e company **fact
+00003170: 732a 2a2e 0a54 6865 2053 4543 2773 2063  s**..The SEC's c
+00003180: 6f6d 7061 6e79 2041 5049 2061 6c73 6f20  ompany API also 
+00003190: 7375 7070 6c69 6573 2061 206c 6f74 206d  supplies a lot m
+000031a0: 6f72 6520 6465 7461 696c 7320 6162 6f75  ore details abou
+000031b0: 7420 6120 636f 6d70 616e 7920 696e 636c  t a company incl
+000031c0: 7564 696e 6720 696e 6475 7374 7279 2c20  uding industry, 
+000031d0: 7468 6520 5345 4320 6669 6c65 7220 7479  the SEC filer ty
+000031e0: 7065 2c0a 7468 6520 6d61 696c 696e 6720  pe,.the mailing 
+000031f0: 616e 6420 6275 7369 6e65 7373 2061 6464  and business add
+00003200: 7265 7373 2061 6e64 206d 7563 6820 6d6f  ress and much mo
+00003210: 7265 2e0a 0a23 2323 2046 696e 6420 6120  re...### Find a 
+00003220: 636f 6d70 616e 7920 7573 696e 6720 7468  company using th
+00003230: 6520 6369 6b0a 5468 6520 2a2a 6369 6b2a  e cik.The **cik*
+00003240: 2a20 6973 2074 6865 2069 6420 7468 6174  * is the id that
+00003250: 2075 6e69 7175 656c 7920 6964 656e 7469   uniquely identi
+00003260: 6669 6573 2061 2063 6f6d 7061 6e79 2061  fies a company a
+00003270: 7420 7468 6520 5345 432e 0a49 7420 6973  t the SEC..It is
+00003280: 2061 206e 756d 6265 722c 2062 7574 2069   a number, but i
+00003290: 7320 736f 6d65 7469 6d65 7320 7368 6f77  s sometimes show
+000032a0: 6e20 696e 2053 4543 2045 6467 6172 2072  n in SEC Edgar r
+000032b0: 6573 6f75 7263 6573 2061 7320 6120 7374  esources as a st
+000032c0: 7269 6e67 2070 6164 6465 6420 7769 7468  ring padded with
+000032d0: 206c 6561 6469 6e67 207a 6572 6f27 732e   leading zero's.
+000032e0: 0a46 6f72 2074 6865 2065 6467 6172 2063  .For the edgar c
+000032f0: 6c69 656e 7420 4150 492c 206a 7573 7420  lient API, just 
+00003300: 7573 6520 7468 6520 6e75 6d62 6572 7320  use the numbers 
+00003310: 616e 6420 6f6d 6974 2074 6865 206c 6561  and omit the lea
+00003320: 6469 6e67 207a 6572 6f65 732e 0a0a 6060  ding zeroes...``
+00003330: 6070 7974 686f 6e0a 636f 6d70 616e 7920  `python.company 
+00003340: 3d20 436f 6d70 616e 7928 3133 3234 3432  = Company(132442
+00003350: 3429 0a60 6060 0a21 5b65 7870 655d 2868  4).```.![expe](h
+00003360: 7474 7073 3a2f 2f72 6177 2e67 6974 6875  ttps://raw.githu
+00003370: 6275 7365 7263 6f6e 7465 6e74 2e63 6f6d  busercontent.com
+00003380: 2f64 6775 6e6e 696e 672f 6564 6761 7274  /dgunning/edgart
+00003390: 6f6f 6c73 2f6d 6169 6e2f 696d 6167 6573  ools/main/images
+000033a0: 2f65 7870 652e 706e 6729 0a0a 0a0a 2323  /expe.png)....##
+000033b0: 2320 4669 6e64 2061 2063 6f6d 7061 6e79  # Find a company
+000033c0: 2075 7369 6e67 2074 6963 6b65 720a 0a59   using ticker..Y
+000033d0: 6f75 2063 616e 2067 6574 2061 2063 6f6d  ou can get a com
+000033e0: 7061 6e79 2075 7369 6e67 2061 2074 6963  pany using a tic
+000033f0: 6b65 7220 652e 672e 202a 2a53 4e4f 572a  ker e.g. **SNOW*
+00003400: 2a2e 2054 6869 7320 7769 6c6c 2064 6f20  *. This will do 
+00003410: 6120 6c6f 6f6b 7570 2066 6f72 2074 6865  a lookup for the
+00003420: 2063 6f6d 7061 6e79 2063 696b 2075 7369   company cik usi
+00003430: 6e67 2074 6865 2074 6963 6b65 722c 2074  ng the ticker, t
+00003440: 6865 6e20 6c6f 6164 2074 6865 2063 6f6d  hen load the com
+00003450: 7061 6e79 2075 7369 6e67 2074 6865 2063  pany using the c
+00003460: 696b 2e0a 5468 6973 206d 616b 6573 2069  ik..This makes i
+00003470: 7420 7477 6f20 6361 6c6c 7320 7665 7273  t two calls vers
+00003480: 7573 206f 6e65 2066 6f72 2074 6865 2063  us one for the c
+00003490: 696b 2063 6f6d 7061 6e79 206c 6f6f 6b75  ik company looku
+000034a0: 702c 2062 7574 2069 7320 736f 6d65 7469  p, but is someti
+000034b0: 6d65 7320 6d6f 7265 2063 6f6e 7665 6e69  mes more conveni
+000034c0: 656e 7420 7369 6e63 6520 7469 636b 6572  ent since ticker
+000034d0: 7320 6172 6520 6561 7369 6572 2074 6f20  s are easier to 
+000034e0: 7265 6d65 6d62 6572 2074 6861 7420 6369  remember that ci
+000034f0: 6b73 2e0a 0a4e 6f74 6520 7468 6174 2073  ks...Note that s
+00003500: 6f6d 6520 636f 6d70 616e 6965 7320 6861  ome companies ha
+00003510: 7665 206d 756c 7469 706c 6520 7469 636b  ve multiple tick
+00003520: 6572 732c 2073 6f20 796f 7520 7465 6368  ers, so you tech
+00003530: 6e69 6361 6c6c 7920 6361 6e6e 6f74 2067  nically cannot g
+00003540: 6574 2053 4543 2066 696c 696e 6773 2066  et SEC filings f
+00003550: 6f72 2061 2074 6963 6b65 722e 0a59 6f75  or a ticker..You
+00003560: 2069 6e73 7465 6164 2067 6574 2074 6865   instead get the
+00003570: 2053 4543 2066 696c 696e 6773 2066 6f72   SEC filings for
+00003580: 2074 6865 2063 6f6d 7061 6e79 2074 6f20   the company to 
+00003590: 7768 6963 6820 7468 6520 7469 636b 6572  which the ticker
+000035a0: 2062 656c 6f6e 6773 2e0a 0a54 6865 2074   belongs...The t
+000035b0: 6963 6b65 7220 6973 2063 6173 652d 696e  icker is case-in
+000035c0: 7365 6e73 6974 6976 6520 736f 2079 6f75  sensitive so you
+000035d0: 2063 616e 2075 7365 2060 436f 6d70 616e   can use `Compan
+000035e0: 7928 2273 6e6f 7722 2960 0a6f 7220 6043  y("snow")`.or `C
+000035f0: 6f6d 7061 6e79 2822 534e 4f57 2229 600a  ompany("SNOW")`.
+00003600: 6060 6070 7974 686f 6e0a 736e 6f77 203d  ```python.snow =
+00003610: 2043 6f6d 7061 6e79 2822 736e 6f77 2229   Company("snow")
+00003620: 0a60 6060 0a0a 215b 736e 6f77 2069 6e73  .```..![snow ins
+00003630: 7065 6374 5d28 6874 7470 733a 2f2f 7261  pect](https://ra
+00003640: 772e 6769 7468 7562 7573 6572 636f 6e74  w.githubusercont
+00003650: 656e 742e 636f 6d2f 6467 756e 6e69 6e67  ent.com/dgunning
+00003660: 2f65 6467 6172 746f 6f6c 732f 6d61 696e  /edgartools/main
+00003670: 2f69 6d61 6765 732f 736e 6f77 2d69 6e73  /images/snow-ins
+00003680: 7065 6374 2e70 6e67 290a 2323 2320 0a0a  pect.png).### ..
+00003690: 0a60 6060 7079 7468 6f6e 0a43 6f6d 7061  .```python.Compa
+000036a0: 6e79 2831 3833 3239 3530 290a 6060 600a  ny(1832950).```.
+000036b0: 0a23 2323 2047 6574 2066 696c 696e 6773  .### Get filings
+000036c0: 2066 6f72 2061 2063 6f6d 7061 6e79 0a54   for a company.T
+000036d0: 6f20 6765 7420 7468 6520 636f 6d70 616e  o get the compan
+000036e0: 7927 7320 6669 6c69 6e67 7320 7573 6520  y's filings use 
+000036f0: 6067 6574 5f66 696c 696e 6773 2829 602e  `get_filings()`.
+00003700: 2054 6869 7320 6765 7473 2061 6c6c 2074   This gets all t
+00003710: 6865 2063 6f6d 7061 6e79 2773 2066 696c  he company's fil
+00003720: 696e 6773 2074 6861 7420 6172 6520 6176  ings that are av
+00003730: 6169 6c61 626c 6520 6672 6f6d 2074 6865  ailable from the
+00003740: 2045 6467 6172 2073 7562 6d69 7373 696f   Edgar submissio
+00003750: 6e73 2065 6e64 706f 696e 742e 0a0a 6060  ns endpoint...``
+00003760: 6070 7974 686f 6e0a 636f 6d70 616e 792e  `python.company.
+00003770: 6765 745f 6669 6c69 6e67 7328 290a 6060  get_filings().``
+00003780: 600a 2323 2320 4669 6c74 6572 696e 6720  `.### Filtering 
+00003790: 6669 6c69 6e67 730a 596f 7520 6361 6e20  filings.You can 
+000037a0: 6669 6c74 6572 2074 6865 2063 6f6d 7061  filter the compa
+000037b0: 6e79 2066 696c 696e 6773 2075 7369 6e67  ny filings using
+000037c0: 2061 206e 756d 6265 7220 6f66 2064 6966   a number of dif
+000037d0: 6665 7265 6e74 2070 6172 616d 6574 6572  ferent parameter
+000037e0: 732e 0a0a 6060 6070 7974 686f 6e0a 636c  s...```python.cl
+000037f0: 6173 7320 436f 6d70 616e 7946 696c 696e  ass CompanyFilin
+00003800: 6773 3a0a 2020 2020 0a20 2020 202e 2e2e  gs:.    .    ...
+00003810: 0a20 2020 200a 2020 2020 6465 6620 6765  .    .    def ge
+00003820: 745f 6669 6c69 6e67 7328 7365 6c66 2c0a  t_filings(self,.
+00003830: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003840: 2020 2020 2a2c 0a20 2020 2020 2020 2020      *,.         
+00003850: 2020 2020 2020 2020 2020 2066 6f72 6d3a             form:
+00003860: 2073 7472 207c 204c 6973 7420 3d20 4e6f   str | List = No
+00003870: 6e65 2c0a 2020 2020 2020 2020 2020 2020  ne,.            
+00003880: 2020 2020 2020 2020 6163 6365 7373 696f          accessio
+00003890: 6e5f 6e75 6d62 6572 3a20 7374 7220 7c20  n_number: str | 
+000038a0: 4c69 7374 203d 204e 6f6e 652c 0a20 2020  List = None,.   
+000038b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000038c0: 2066 696c 655f 6e75 6d62 6572 3a20 7374   file_number: st
+000038d0: 7220 7c20 4c69 7374 203d 204e 6f6e 652c  r | List = None,
+000038e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000038f0: 2020 2020 2069 735f 7862 726c 3a20 626f       is_xbrl: bo
+00003900: 6f6c 203d 204e 6f6e 652c 0a20 2020 2020  ol = None,.     
+00003910: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00003920: 735f 696e 6c69 6e65 5f78 6272 6c3a 2062  s_inline_xbrl: b
+00003930: 6f6f 6c20 3d20 4e6f 6e65 0a20 2020 2020  ool = None.     
+00003940: 2020 2020 2020 2020 2020 2020 2020 2029                 )
+00003950: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
+00003960: 2020 2020 2020 4765 7420 7468 6520 636f        Get the co
+00003970: 6d70 616e 7927 7320 6669 6c69 6e67 7320  mpany's filings 
+00003980: 616e 6420 6f70 7469 6f6e 616c 6c79 2066  and optionally f
+00003990: 696c 7465 7220 6279 206d 756c 7469 706c  ilter by multipl
+000039a0: 6520 6372 6974 6572 6961 0a20 2020 2020  e criteria.     
+000039b0: 2020 203a 7061 7261 6d20 666f 726d 3a20     :param form: 
+000039c0: 5468 6520 666f 726d 2061 7320 6120 7374  The form as a st
+000039d0: 7269 6e67 2065 2e67 2e20 2731 302d 4b27  ring e.g. '10-K'
+000039e0: 206f 7220 4c69 7374 206f 6620 7374 7269   or List of stri
+000039f0: 6e67 7320 5b27 3130 2d51 272c 2027 3130  ngs ['10-Q', '10
+00003a00: 2d4b 275d 0a20 2020 2020 2020 203a 7061  -K'].        :pa
+00003a10: 7261 6d20 6163 6365 7373 696f 6e5f 6e75  ram accession_nu
+00003a20: 6d62 6572 3a20 5468 6520 6163 6365 7373  mber: The access
+00003a30: 696f 6e20 6e75 6d62 6572 2074 6861 7420  ion number that 
+00003a40: 756e 6971 7565 6c79 2069 6465 6e74 6966  uniquely identif
+00003a50: 6965 7320 616e 2053 4543 2066 696c 696e  ies an SEC filin
+00003a60: 6720 652e 672e 2030 3030 3136 3430 3134  g e.g. 000164014
+00003a70: 372d 3232 2d30 3030 3130 300a 2020 2020  7-22-000100.    
+00003a80: 2020 2020 3a70 6172 616d 2066 696c 655f      :param file_
+00003a90: 6e75 6d62 6572 3a20 5468 6520 6669 6c65  number: The file
+00003aa0: 206e 756d 6265 7220 652e 672e 2030 3031   number e.g. 001
+00003ab0: 2d33 3935 3034 0a20 2020 2020 2020 203a  -39504.        :
+00003ac0: 7061 7261 6d20 6973 5f78 6272 6c3a 2057  param is_xbrl: W
+00003ad0: 6865 7468 6572 2074 6865 2066 696c 696e  hether the filin
+00003ae0: 6720 6973 2078 6272 6c0a 2020 2020 2020  g is xbrl.      
+00003af0: 2020 3a70 6172 616d 2069 735f 696e 6c69    :param is_inli
+00003b00: 6e65 5f78 6272 6c3a 2057 6865 7468 6572  ne_xbrl: Whether
+00003b10: 2074 6865 2066 696c 696e 6720 6973 2069   the filing is i
+00003b20: 6e6c 696e 655f 7862 726c 0a20 2020 2020  nline_xbrl.     
+00003b30: 2020 203a 7265 7475 726e 3a20 5468 6520     :return: The 
+00003b40: 436f 6d70 616e 7946 696c 696e 6720 696e  CompanyFiling in
+00003b50: 7374 616e 6365 2077 6974 6820 7468 6520  stance with the 
+00003b60: 6669 6c69 6e67 7320 7468 6174 206d 6174  filings that mat
+00003b70: 6368 2074 6865 2066 696c 7465 7273 0a20  ch the filters. 
+00003b80: 2020 2020 2020 2022 2222 0a60 6060 0a0a         """.```..
+00003b90: 0a23 2323 2320 5468 6520 436f 6d70 616e  .#### The Compan
+00003ba0: 7946 696c 696e 6773 2063 6c61 7373 0a54  yFilings class.T
+00003bb0: 6865 2072 6573 756c 7420 6f66 2060 6765  he result of `ge
+00003bc0: 745f 6669 6c69 6e67 7328 2960 2069 7320  t_filings()` is 
+00003bd0: 6120 6043 6f6d 7061 6e79 4669 6c69 6e67  a `CompanyFiling
+00003be0: 7360 2063 6c61 7373 2e20 5468 6973 2063  s` class. This c
+00003bf0: 6c61 7373 2063 6f6e 7461 696e 7320 6120  lass contains a 
+00003c00: 7079 6172 726f 7720 7461 626c 6520 7769  pyarrow table wi
+00003c10: 7468 2074 6865 2066 696c 696e 6773 0a61  th the filings.a
+00003c20: 6e64 2070 726f 7669 6465 7320 636f 6e76  nd provides conv
+00003c30: 656e 6965 6e74 2066 756e 6374 696f 6e73  enient functions
+00003c40: 2066 6f72 2077 6f72 6b69 6e67 2077 6974   for working wit
+00003c50: 6820 6669 6c69 6e67 732e 0a59 6f75 2063  h filings..You c
+00003c60: 616e 2061 6363 6573 7320 7468 6520 756e  an access the un
+00003c70: 6465 726c 7969 6e67 2070 7961 7272 6f77  derlying pyarrow
+00003c80: 2060 5461 626c 6560 2075 7369 6e67 2074   `Table` using t
+00003c90: 6865 2060 2e64 6174 6160 2070 726f 7065  he `.data` prope
+00003ca0: 7274 790a 0a60 6060 7079 7468 6f6e 0a66  rty..```python.f
+00003cb0: 696c 696e 6773 203d 2063 6f6d 7061 6e79  ilings = company
+00003cc0: 2e67 6574 5f66 696c 696e 6773 2829 0a0a  .get_filings()..
+00003cd0: 2320 4765 7420 7468 6520 756e 6465 726c  # Get the underl
+00003ce0: 7969 6e67 2054 6162 6c65 0a64 6174 613a  ying Table.data:
+00003cf0: 2070 612e 5461 626c 6520 3d20 6669 6c69   pa.Table = fili
+00003d00: 6e67 732e 6461 7461 0a60 6060 0a0a 2323  ngs.data.```..##
+00003d10: 2323 2047 6574 2061 2066 696c 696e 6720  ## Get a filing 
+00003d20: 6279 2069 6e64 6578 0a54 6f20 6163 6365  by index.To acce
+00003d30: 7373 2061 2066 696c 696e 6720 696e 2074  ss a filing in t
+00003d40: 6865 2043 6f6d 7061 6e79 4669 6c69 6e67  he CompanyFiling
+00003d50: 7320 7573 6520 7468 6520 6272 6163 6b65  s use the bracke
+00003d60: 7420 605b 5d60 206e 6f74 6174 696f 6e20  t `[]` notation 
+00003d70: 652e 672e 2060 6669 6c69 6e67 735b 325d  e.g. `filings[2]
+00003d80: 600a 6060 6070 7974 686f 6e0a 6669 6c69  `.```python.fili
+00003d90: 6e67 735b 325d 0a60 6060 0a0a 2323 2323  ngs[2].```..####
+00003da0: 2047 6574 2074 6865 206c 6174 6573 7420   Get the latest 
+00003db0: 6669 6c69 6e67 0a0a 5468 6520 6043 6f6d  filing..The `Com
+00003dc0: 7061 6e79 4669 6c69 6e67 7360 2063 6c61  panyFilings` cla
+00003dd0: 7373 2068 6173 2061 2060 6c61 7465 7374  ss has a `latest
+00003de0: 6020 6675 6e63 7469 6f6e 2074 6861 7420  ` function that 
+00003df0: 7769 6c6c 2072 6574 7572 6e20 7468 6520  will return the 
+00003e00: 6c61 7465 7374 2060 4669 6c69 6e67 602e  latest `Filing`.
+00003e10: 200a 536f 2c20 746f 2067 6574 2074 6865   .So, to get the
+00003e20: 206c 6174 6573 7420 2a2a 3130 2d51 2a2a   latest **10-Q**
+00003e30: 2066 696c 696e 672c 2079 6f75 2064 6f20   filing, you do 
+00003e40: 7468 6520 666f 6c6c 6f77 696e 670a 6060  the following.``
+00003e50: 6070 7974 686f 6e0a 2320 4c61 7465 7374  `python.# Latest
+00003e60: 2066 696c 696e 6720 6d61 6b65 7320 7365   filing makes se
+00003e70: 6e73 6520 6966 2079 6f75 2066 696c 7465  nse if you filte
+00003e80: 7220 6279 2066 6f72 6d20 2074 7970 6520  r by form  type 
+00003e90: 652e 672e 2031 302d 510a 736e 6f77 5f31  e.g. 10-Q.snow_1
+00003ea0: 3051 7320 3d20 736e 6f77 2e67 6574 5f66  0Qs = snow.get_f
+00003eb0: 696c 696e 6773 2866 6f72 6d3d 2731 302d  ilings(form='10-
+00003ec0: 5127 290a 6c61 7465 7374 5f31 3051 203d  Q').latest_10Q =
+00003ed0: 2073 6e6f 775f 3130 5173 2e6c 6174 6573   snow_10Qs.lates
+00003ee0: 7428 290a 0a23 204f 7220 6368 6169 6e20  t()..# Or chain 
+00003ef0: 7468 6520 6675 6e63 7469 6f6e 2063 616c  the function cal
+00003f00: 6c73 0a73 6e6f 772e 6765 745f 6669 6c69  ls.snow.get_fili
+00003f10: 6e67 7328 666f 726d 3d27 3130 2d51 2729  ngs(form='10-Q')
+00003f20: 2e6c 6174 6573 7428 290a 6060 600a 0a0a  .latest().```...
+00003f30: 2323 2320 4765 7420 636f 6d70 616e 7920  ### Get company 
+00003f40: 6661 6374 730a 0a46 6163 7473 2061 7265  facts..Facts are
+00003f50: 2061 6e20 696e 7465 7265 7374 696e 6720   an interesting 
+00003f60: 616e 6420 696d 706f 7274 616e 7420 6461  and important da
+00003f70: 7461 7365 7420 6162 6f75 7420 6120 636f  taset about a co
+00003f80: 6d70 616e 7920 6163 6375 6d6c 6174 6564  mpany accumlated
+00003f90: 2066 726f 6d20 6461 7461 2074 6865 2063   from data the c
+00003fa0: 6f6d 7061 6e79 2070 726f 7669 6465 7320  ompany provides 
+00003fb0: 746f 2074 6865 2053 4543 2e0a 436f 6d70  to the SEC..Comp
+00003fc0: 616e 7920 6661 6374 7320 6172 6520 6176  any facts are av
+00003fd0: 6169 6c61 626c 6520 666f 7220 6120 636f  ailable for a co
+00003fe0: 6d70 616e 7920 6f6e 2074 6865 2043 6f6d  mpany on the Com
+00003ff0: 7061 6e79 2046 6163 7473 6066 2268 7474  pany Facts`f"htt
+00004000: 7073 3a2f 2f64 6174 612e 7365 632e 676f  ps://data.sec.go
+00004010: 762f 6170 692f 7862 726c 2f63 6f6d 7061  v/api/xbrl/compa
+00004020: 6e79 6661 6374 732f 4349 4b7b 6369 6b3a  nyfacts/CIK{cik:
+00004030: 3031 307d 2e6a 736f 6e22 600a 4974 2069  010}.json"`.It i
+00004040: 7320 6120 4a53 4f4e 2065 6e64 706f 696e  s a JSON endpoin
+00004050: 7420 616e 6420 6065 6467 6172 746f 6f6c  t and `edgartool
+00004060: 7360 2070 6172 7365 7320 7468 6520 4a53  s` parses the JS
+00004070: 4f4e 2069 6e74 6f20 6120 7374 7275 6374  ON into a struct
+00004080: 7572 6564 2064 6174 6173 6574 202d 2061  ured dataset - a
+00004090: 2060 7079 6172 726f 772e 5461 626c 6560   `pyarrow.Table`
+000040a0: 2e0a 0a23 2323 2320 4765 7474 696e 6720  ...#### Getting 
+000040b0: 6661 6374 7320 666f 7220 6120 636f 6d70  facts for a comp
+000040c0: 616e 790a 546f 2067 6574 2063 6f6d 7061  any.To get compa
+000040d0: 6e79 2066 6163 7473 2c20 6669 7273 7420  ny facts, first 
+000040e0: 6765 7420 7468 6520 636f 6d70 616e 792c  get the company,
+000040f0: 2074 6865 6e20 6361 6c6c 2060 636f 6d70   then call `comp
+00004100: 616e 792e 6765 745f 6661 6374 7328 2960  any.get_facts()`
+00004110: 0a60 6060 7079 7468 6f6e 0a63 6f6d 7061  .```python.compa
+00004120: 6e79 203d 2043 6f6d 7061 6e79 2822 534e  ny = Company("SN
+00004130: 4f57 2229 0a63 6f6d 7061 6e79 5f66 6163  OW").company_fac
+00004140: 7473 203d 2063 6f6d 7061 6e79 2e67 6574  ts = company.get
+00004150: 5f66 6163 7473 2829 0a60 6060 0a54 6865  _facts().```.The
+00004160: 2072 6573 756c 7420 6973 2061 2060 436f   result is a `Co
+00004170: 6d70 616e 7946 6163 7473 6020 6f62 6a65  mpanyFacts` obje
+00004180: 6374 2077 6869 6368 2077 7261 7073 2074  ct which wraps t
+00004190: 6865 2075 6e64 6572 6c79 696e 6720 6661  he underlying fa
+000041a0: 6374 7320 616e 6420 7072 6f76 6964 6573  cts and provides
+000041b0: 2063 6f6e 7665 6e69 656e 7420 7761 7973   convenient ways
+000041c0: 206f 6620 776f 726b 696e 670a 7769 7468   of working.with
+000041d0: 2074 6865 2066 6163 7473 2064 6174 612e   the facts data.
+000041e0: 2054 6f20 6765 7420 6163 6365 7373 2074   To get access t
+000041f0: 6f20 7468 6520 756e 6465 7279 6c69 6e67  o the underyling
+00004200: 2064 6174 6120 7573 6520 7468 6520 6066   data use the `f
+00004210: 6163 7473 6020 7072 6f70 6572 7479 2e0a  acts` property..
+00004220: 0a59 6f75 2063 616e 2067 6574 2074 6865  .You can get the
+00004230: 2066 6163 7473 2061 7320 6120 7061 6e64   facts as a pand
+00004240: 6173 2064 6174 6166 7261 6d65 2062 7920  as dataframe by 
+00004250: 6361 6c6c 696e 6720 6074 6f5f 7061 6e64  calling `to_pand
+00004260: 6173 600a 0a60 6060 7079 7468 6f6e 0a64  as`..```python.d
+00004270: 6620 3d20 636f 6d70 616e 795f 6661 6374  f = company_fact
+00004280: 732e 746f 5f70 616e 6461 7328 290a 6060  s.to_pandas().``
+00004290: 600a 0a46 6163 7473 2064 6966 6665 7220  `..Facts differ 
+000042a0: 616d 6f6e 6720 636f 6d70 616e 6965 732e  among companies.
+000042b0: 2054 6f20 7365 6520 7768 6174 2066 6163   To see what fac
+000042c0: 7473 2061 7265 2061 7661 696c 6162 6c65  ts are available
+000042d0: 2079 6f75 2063 616e 2075 7365 2074 6865   you can use the
+000042e0: 2060 6661 6374 735f 6d65 7461 6020 7072   `facts_meta` pr
+000042f0: 6f70 6572 7479 2e0a 0a23 2323 2320 4765  operty...#### Ge
+00004300: 7474 696e 6720 7468 6520 6661 6374 7320  tting the facts 
+00004310: 6173 2061 2044 7563 6b44 4220 7461 626c  as a DuckDB tabl
+00004320: 650a 5970 7520 6361 6e20 636f 6e76 6572  e.Ypu can conver
+00004330: 7420 7468 6520 6661 6374 7320 746f 2061  t the facts to a
+00004340: 2044 7563 6b44 4220 6461 7461 6261 7365   DuckDB database
+00004350: 2077 6869 6368 2061 6c6c 6f77 7320 796f   which allows yo
+00004360: 7520 746f 2071 7565 7279 2074 6865 2066  u to query the f
+00004370: 6163 7473 2075 7369 6e67 2053 514c 2e0a  acts using SQL..
+00004380: 0a60 6060 7079 7468 6f6e 0a20 2020 2063  .```python.    c
+00004390: 6f6d 7061 6e79 5f66 6163 7473 3a20 436f  ompany_facts: Co
+000043a0: 6d70 616e 7946 6163 7473 203d 2067 6574  mpanyFacts = get
+000043b0: 5f63 6f6d 7061 6e79 5f66 6163 7473 2831  _company_facts(1
+000043c0: 3331 3836 3035 290a 2020 2020 6462 203d  318605).    db =
+000043d0: 2063 6f6d 7061 6e79 5f66 6163 7473 2e74   company_facts.t
+000043e0: 6f5f 6475 636b 6462 2829 0a20 2020 2064  o_duckdb().    d
+000043f0: 6620 3d20 6462 2e65 7865 6375 7465 2822  f = db.execute("
+00004400: 2222 0a20 2020 2073 656c 6563 7420 2a20  "".    select * 
+00004410: 6672 6f6d 2066 6163 7473 0a20 2020 2022  from facts.    "
+00004420: 2222 292e 6466 2829 0a60 6060 0a0a 0a0a  "").df().```....
+00004430: 2320 436f 6e74 7269 6275 7469 6e67 0a0a  # Contributing..
+00004440: 436f 6e74 7269 6275 7469 6f6e 7320 6172  Contributions ar
+00004450: 6520 7765 6c63 6f6d 6521 2057 6520 776f  e welcome! We wo
+00004460: 756c 6420 6c6f 7665 2074 6f20 6865 6172  uld love to hear
+00004470: 2079 6f75 7220 7468 6f75 6768 7473 206f   your thoughts o
+00004480: 6e20 686f 7720 7468 6973 206c 6962 7261  n how this libra
+00004490: 7279 2063 6f75 6c64 2062 6520 6265 7474  ry could be bett
+000044a0: 6572 2061 7420 776f 726b 696e 6720 7769  er at working wi
+000044b0: 7468 2053 4543 2045 6467 6172 2e0a 0a23  th SEC Edgar...#
+000044c0: 2320 5265 706f 7274 696e 6720 4973 7375  # Reporting Issu
+000044d0: 6573 0a57 6520 7573 6520 4769 7448 7562  es.We use GitHub
+000044e0: 2069 7373 7565 7320 746f 2074 7261 636b   issues to track
+000044f0: 2070 7562 6c69 6320 6275 6773 2e20 0a52   public bugs. .R
+00004500: 6570 6f72 7420 6120 6275 6720 6279 205b  eport a bug by [
+00004510: 6f70 656e 696e 6720 6120 6e65 7720 6973  opening a new is
+00004520: 7375 655d 2868 7474 7073 3a2f 2f67 6974  sue](https://git
+00004530: 6875 622e 636f 6d2f 6467 756e 6e69 6e67  hub.com/dgunning
+00004540: 2f65 6467 6172 746f 6f6c 732f 6973 7375  /edgartools/issu
+00004550: 6573 293b 2069 7427 7320 7468 6174 2065  es); it's that e
+00004560: 6173 7921 0a0a 2323 204d 616b 696e 6720  asy!..## Making 
+00004570: 636f 6465 2063 6861 6e67 6573 0a2d 2046  code changes.- F
+00004580: 6f72 6b20 7468 6520 7265 706f 2061 6e64  ork the repo and
+00004590: 2063 7265 6174 6520 796f 7572 2062 7261   create your bra
+000045a0: 6e63 6820 6672 6f6d 206d 6173 7465 722e  nch from master.
+000045b0: 0a2d 2049 6620 796f 7527 7665 2061 6464  .- If you've add
+000045c0: 6564 2063 6f64 6520 7468 6174 2073 686f  ed code that sho
+000045d0: 756c 6420 6265 2074 6573 7465 642c 2061  uld be tested, a
+000045e0: 6464 2074 6573 7473 2e0a 2d20 4966 2079  dd tests..- If y
+000045f0: 6f75 2776 6520 6368 616e 6765 6420 4150  ou've changed AP
+00004600: 4973 2c20 7570 6461 7465 2074 6865 2064  Is, update the d
+00004610: 6f63 756d 656e 7461 7469 6f6e 2e0a 2d20  ocumentation..- 
+00004620: 456e 7375 7265 2074 6865 2074 6573 7420  Ensure the test 
+00004630: 7375 6974 6520 7061 7373 6573 2e0a 2d20  suite passes..- 
+00004640: 4d61 6b65 2073 7572 6520 796f 7572 2063  Make sure your c
+00004650: 6f64 6520 6c69 6e74 732e 0a2d 2049 7373  ode lints..- Iss
+00004660: 7565 2074 6861 7420 7075 6c6c 2072 6571  ue that pull req
+00004670: 7565 7374 210a 0a0a 0a23 204c 6963 656e  uest!....# Licen
+00004680: 7365 0a0a 6065 6467 6172 746f 6f6c 7360  se..`edgartools`
+00004690: 2069 7320 6469 7374 7269 6275 7465 6420   is distributed 
+000046a0: 756e 6465 7220 7468 6520 7465 726d 7320  under the terms 
+000046b0: 6f66 2074 6865 205b 4d49 545d 2868 7474  of the [MIT](htt
+000046c0: 7073 3a2f 2f73 7064 782e 6f72 672f 6c69  ps://spdx.org/li
+000046d0: 6365 6e73 6573 2f4d 4954 2e68 746d 6c29  censes/MIT.html)
+000046e0: 206c 6963 656e 7365 2e0a 0a23 2320 436f   license...## Co
+000046f0: 6e74 6163 740a 0a5b 4c69 6e6b 6564 496e  ntact..[LinkedIn
+00004700: 5d28 6874 7470 733a 2f2f 7777 772e 6c69  ](https://www.li
+00004710: 6e6b 6564 696e 2e63 6f6d 2f69 6e2f 6477  nkedin.com/in/dw
+00004720: 6967 6874 2d67 756e 6e69 6e67 2d38 3630  ight-gunning-860
+00004730: 3132 342f 29                             124/)
```

