# Walmart Store Sales Forecasting
## Introduction
Walmart is an American multinational retail corporation that operates a chain of supermarkets, discount department stores, and grocery stores. The company was founded by Sam Walton in 1962 and incorporated on October 31, 1969.

## Problem Statement
We have access to historical sales data for 45 Walmart locations around the country. The goal is to project department-wide sales for each store based on the available data.

## Data Overview
There are four datasets available in the data:

* `stores.csv`: Contains anonymized information about the 45 stores, including the type and size of the store.

* `train.csv`: Historical training data covering the period from 2010-02-05 to 2012-11-01. 
The following fields are available in this file:

 - `Store`: Store number
 - `Dept`: Department number
 - `Date`: Week
 - `Weekly_Sales`: Sales for the given department in the given store
 - `IsHoliday`: Whether the week is a special holiday week
* `test.csv`: Identical to the `train.csv` file, except the weekly sales are withheld. The sales must be predicted for each store, department, and date in this file.

* `features.csv`: Contains additional data related to the store, department, and regional activity for the given dates. The following fields are available:

 - `Store`: Store number
 - `Date`: Week
 - `Temperature`: Average temperature in the region
 - `Fuel_Price`: Cost of fuel in the region
 - `MarkDown1-5`: Anonymized data related to promotional markdowns that Walmart is running. Markdown data is only available after November 2011 and is not available for all stores all the time. Any missing value is marked with an NA.
 - `CPI`: Consumer price index
 - `Unemployment`: Unemployment rate
 - `IsHoliday`: Whether the week is a special holiday week
