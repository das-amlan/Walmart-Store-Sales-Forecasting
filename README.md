# Walmart-Store-Sales-Forecasting
Walmart is an American global retail firm headquartered in Bentonville, Arkansas, that operates a chain of super markets, cheap department stores, and grocery stores. Sam Walton created the corporation in 1962, and it was incorporated on October 31, 1969.

## Problem
We have access to historical sales data for 45 Walmart locations around the country. Each store has several departments, and we are tasked with projecting department-wide sales for each store.

## Overview of Data
There are a total of four datasets in the data.

1. **stores.csv**

>This file contains anonymized information about the 45 stores, indicating the type and size of store.

2. **train.csv**

>This is the historical training data, which covers to 2010-02-05 to 2012-11-01. Within this file you will find the following fields:

* Store - the store number
* Dept - the department number
* Date - the week
* Weekly_Sales -  sales for the given department in the given store
* IsHoliday - whether the week is a special holiday week

3. **test.csv**

>This file is identical to train.csv, except we have withheld the weekly sales. You must predict the sales for each triplet of store, department, and date in this file.

4. **features.csv**

>This file contains additional data related to the store, department, and regional activity for the given dates. It contains the following fields:

* Store - the store number
* Date - the week
* Temperature - average temperature in the region
* Fuel_Price - cost of fuel in the region
* MarkDown1-5 - anonymized data related to promotional markdowns that Walmart is running. MarkDown data is only available after Nov 2011, and is not available for all stores all the time. Any missing value is marked with an NA.
* CPI - the consumer price index
* Unemployment - the unemployment rate
* IsHoliday - whether the week is a special holiday week
