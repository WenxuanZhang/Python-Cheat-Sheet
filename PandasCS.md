Pandas
----------------
Pandas is a python library that provide providing fast, flexible, and expressive data structures designed to make working with “relational” or “labeled” data both easy and intuitive.

Read in Data
----------------
Pandas is able to read Data in various format,such as 
+ Yahoo Finance 
+ Google Finance
+ St Louis Fed
+ Kenneth French's data Library
+ World Bank 
+ Google Analytics
[details](http://pandas.pydata.org/pandas-docs/version/0.15.2/remote_data.html#remote-data-fred)
+ CSV
+ excel
+ hdf
+ sql
+ json
+ clipborad
+ pickle
+ stata
```python
import pandas as pd
pd.read_csv()

```
Create DataFrame
----------------
```python
import pandas as pd
import numpy as np
# create series
s = pd.Series([1,3,5,np.nan,6,8])
name = pd.Series(['a','b','c','d','e','f'])
# create dataframe
example = pd.DataFrame({"name":name,"score":s,"index":[range(0,len(s))]})
# create index 
example.index= map(str,range(0,len(s)))
# access index
example.loc["3","score"]
```
Access DataFrame
----------------
```python
# access by index 
#  Index Based Accessing
example.loc["3":"4","score"]
# Location Based Accessing

# Condition Based Accessing

# 
```


Merge DataFrame 
---------------

