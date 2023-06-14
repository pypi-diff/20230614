# Comparing `tmp/volvisualizer-1.1.1-py3-none-any.whl.zip` & `tmp/volvisualizer-1.1.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 26951 bytes, number of entries: 13
--rw-rw-rw-  2.0 fat       31 b- defN 23-Jan-06 09:25 volvisualizer/__init__.py
+Zip file size: 27328 bytes, number of entries: 13
+-rw-rw-rw-  2.0 fat       23 b- defN 23-Jun-14 14:38 volvisualizer/__init__.py
 -rw-rw-rw-  2.0 fat    26576 b- defN 22-Mar-16 10:04 volvisualizer/graph.py
--rw-rw-rw-  2.0 fat    12086 b- defN 22-Mar-30 07:28 volvisualizer/market_data.py
--rw-rw-rw-  2.0 fat    25065 b- defN 22-Mar-16 09:22 volvisualizer/market_data_prep.py
+-rw-rw-rw-  2.0 fat    11866 b- defN 23-Jun-14 14:40 volvisualizer/market_data.py
+-rw-rw-rw-  2.0 fat    25959 b- defN 23-Jun-14 14:48 volvisualizer/market_data_prep.py
 -rw-rw-rw-  2.0 fat     2857 b- defN 22-Mar-16 09:22 volvisualizer/utils.py
 -rw-rw-rw-  2.0 fat    30001 b- defN 22-Mar-15 16:13 volvisualizer/vol_methods.py
 -rw-rw-rw-  2.0 fat    13496 b- defN 22-Mar-16 09:22 volvisualizer/volatility.py
--rw-rw-rw-  2.0 fat     3009 b- defN 22-Mar-09 16:51 volvisualizer/volatility_params.py
--rw-rw-rw-  2.0 fat     1089 b- defN 23-Jan-06 09:32 volvisualizer-1.1.1.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      694 b- defN 23-Jan-06 09:32 volvisualizer-1.1.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jan-06 09:32 volvisualizer-1.1.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       14 b- defN 23-Jan-06 09:32 volvisualizer-1.1.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     1093 b- defN 23-Jan-06 09:32 volvisualizer-1.1.1.dist-info/RECORD
-13 files, 116103 bytes uncompressed, 25125 bytes compressed:  78.4%
+-rw-rw-rw-  2.0 fat     3914 b- defN 23-Jun-14 14:38 volvisualizer/volatility_params.py
+-rw-rw-rw-  2.0 fat     1089 b- defN 23-Jun-14 14:58 volvisualizer-1.1.2.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      727 b- defN 23-Jun-14 14:58 volvisualizer-1.1.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-14 14:58 volvisualizer-1.1.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       14 b- defN 23-Jun-14 14:58 volvisualizer-1.1.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1093 b- defN 23-Jun-14 14:58 volvisualizer-1.1.2.dist-info/RECORD
+13 files, 117707 bytes uncompressed, 25502 bytes compressed:  78.3%
```

## zipnote {}

```diff
@@ -18,23 +18,23 @@
 
 Filename: volvisualizer/volatility.py
 Comment: 
 
 Filename: volvisualizer/volatility_params.py
 Comment: 
 
-Filename: volvisualizer-1.1.1.dist-info/LICENSE
+Filename: volvisualizer-1.1.2.dist-info/LICENSE
 Comment: 
 
-Filename: volvisualizer-1.1.1.dist-info/METADATA
+Filename: volvisualizer-1.1.2.dist-info/METADATA
 Comment: 
 
-Filename: volvisualizer-1.1.1.dist-info/WHEEL
+Filename: volvisualizer-1.1.2.dist-info/WHEEL
 Comment: 
 
-Filename: volvisualizer-1.1.1.dist-info/top_level.txt
+Filename: volvisualizer-1.1.2.dist-info/top_level.txt
 Comment: 
 
-Filename: volvisualizer-1.1.1.dist-info/RECORD
+Filename: volvisualizer-1.1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## volvisualizer/__init__.py

```diff
@@ -1,5 +1 @@
-__version__ = "1.1.1"
-
-
-
-
+__version__ = "1.1.2"
```

## volvisualizer/market_data.py

```diff
@@ -1,33 +1,23 @@
 """
 Market data import and transformation functions
 
 """
 import copy
 from datetime import date, timedelta
 import time
-from urllib.request import FancyURLopener
 import warnings
 import datetime as dt
 from bs4 import BeautifulSoup
 import pandas as pd
 from pandas.tseries.holiday import get_calendar, HolidayCalendarFactory, GoodFriday
-from volvisualizer.market_data_prep import DataPrep
+from volvisualizer.market_data_prep import DataPrep, UrlOpener
 warnings.filterwarnings("ignore", category=DeprecationWarning)
 # pylint: disable=invalid-name
 
-# Class used to open urls for financial data
-class UrlOpener(FancyURLopener):
-    """
-    Extract data from Yahoo Finance URL
-
-    """
-    version = 'w3m/0.5.3+git20180125'
-
-
 class Data():
     """
     Market data import and transformation functions
 
     """
     @classmethod
     def create_option_data(cls, params, tables):
@@ -175,15 +165,15 @@
             +'/options?p='+params['ticker']
 
         # Create a UrlOpener object to extract data from the url
         urlopener = UrlOpener()
         response = urlopener.open(url)
 
         # Collect the text from this object
-        params['html_doc'] = response.read()
+        params['html_doc'] = response.text
 
         # Use Beautiful Soup to parse this
         soup = BeautifulSoup(params['html_doc'], features="lxml")
 
         # Create a list of all the option dates
         option_dates = [a.get_text() for a in soup.find_all('option')]
 
@@ -226,15 +216,15 @@
         # it in the url dict
         for input_date, url in params['url_dict'].items():
 
             # UrlOpener function downloads the data
             urlopener = UrlOpener()
             weburl = urlopener.open(url)
             try:
-                raw_web_data[input_date] = weburl.read()
+                raw_web_data[input_date] = weburl.text
 
                 # wait between each query so as not to overload server
                 time.sleep(params['wait'])
 
             # If there is a problem, report the date and apply extended wait
             except ValueError:
                 print("Problem with "+input_date+" data")
```

## volvisualizer/market_data_prep.py

```diff
@@ -3,34 +3,68 @@
 
 """
 import calendar
 from collections import Counter
 import copy
 import datetime as dt
 from datetime import date, timedelta
-from urllib.request import FancyURLopener
+import random
 import warnings
 from lxml import html
 import numpy as np
 import pandas as pd
 import pytz
+import requests
 from scipy import interpolate
 from volvisualizer.vol_methods import ImpliedVol
-
+from volvisualizer.volatility_params import USER_AGENTS
 
 warnings.filterwarnings("ignore", category=DeprecationWarning)
 # pylint: disable=invalid-name
 
-# Class used to open urls for financial data
-class UrlOpener(FancyURLopener):
+
+class UrlOpener:
     """
     Extract data from Yahoo Finance URL
 
     """
-    version = 'w3m/0.5.3+git20180125'
+    request_headers = {
+        "accept": "*/*",
+        "accept-encoding": "gzip, deflate, br",
+        "accept-language": "en-US,en;q=0.9",
+        "origin": "https://finance.yahoo.com",
+        "referer": "https://finance.yahoo.com",
+        "sec-fetch-dest": "empty",
+        "sec-fetch-mode": "cors",
+        "sec-fetch-site": "same-site",
+    }
+    user_agent = random.choice(USER_AGENTS)
+    request_headers["User-Agent"] = user_agent
+
+    def __init__(self):
+        self._session = requests
+
+    def open(self, url):
+        """
+        Extract data from Yahoo Finance URL
+
+        Parameters
+        ----------
+        url : Str
+            The URL to extract data from.
+
+        Returns
+        -------
+        response : Response object
+            Response object of requests module.
+
+        """
+        response = self._session.get(url=url, headers=self.request_headers)
+        
+        return response
 
 
 class DataPrep():
     """
     Market data transformation and combination functions
 
     """
@@ -731,30 +765,30 @@
     def _stock_dividend_yield(ticker):
 
         url = 'https://ycharts.com/companies/'+ticker+'/dividend_yield'
 
         urlopener = UrlOpener()
         response = urlopener.open(url)
 
-        html_doc = response.read()
+        html_doc = response.text
 
         data = pd.read_html(html_doc)
 
         return data[0]['Value'][0]
 
 
     @staticmethod
     def _spx_div_yield():
 
         url = 'https://www.multpl.com/s-p-500-dividend-yield'
 
         urlopener = UrlOpener()
         response = urlopener.open(url)
 
-        html_doc = response.read()
+        html_doc = response.text
 
         tree = html.fromstring(html_doc)
 
         parse = tree.xpath(
             '//div[@id="current"]/text()')
 
         return [str(p) for p in parse][1].replace('\n','')
```

## volvisualizer/volatility_params.py

```diff
@@ -117,7 +117,21 @@
         'axes.edgecolor':'w',
         'lines.linewidth':0.5,
         'xtick.labelbottom':True,
         'ytick.labelleft':True
         },
 
     }
+
+USER_AGENTS = [
+    "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/81.0.4044.138 "
+    "Safari/537.36",
+    "Mozilla/5.0 (Windows NT 10.0; WOW64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/81.0.4044.138 Safari/537.36",
+    "Mozilla/5.0 (Windows NT 10.0) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/81.0.4044.138 Safari/537.36",
+    'Mozilla/5.0 (Macintosh; Intel Mac OS X 10_10_1) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/39.0.2171.95 '
+    'Safari/537.36'
+    "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/81.0.4044.129 "
+    "Safari/537.36",
+    "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_4) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/81.0.4044.138 "
+    "Safari/537.36",
+    "Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/81.0.4044.138 Safari/537.36",
+]
```

## Comparing `volvisualizer-1.1.1.dist-info/LICENSE` & `volvisualizer-1.1.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `volvisualizer-1.1.1.dist-info/METADATA` & `volvisualizer-1.1.2.dist-info/METADATA`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: volvisualizer
-Version: 1.1.1
+Version: 1.1.2
 Summary: Extract and visualize implied volatility from option data.
 Home-page: https://github.com/GBERESEARCH/volvisualizer
 Author: GBERESEARCH
 Author-email: gberesearch@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -12,11 +12,12 @@
 Requires-Dist: scipy (>=1.4.1)
 Requires-Dist: pytz (>=2018.9)
 Requires-Dist: pandas (>=1.0.0)
 Requires-Dist: matplotlib (>=3.0.3)
 Requires-Dist: plotly (>=4.3.0)
 Requires-Dist: beautifulsoup4 (>=4.7.1)
 Requires-Dist: lxml (>=4.3.2)
+Requires-Dist: html5lib (>=1.1)
 
 ## volvisualizer
 
 ### Extract and visualize implied volatility from Yahoo Finance option data.
```

