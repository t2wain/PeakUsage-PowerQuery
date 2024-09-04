## Excel Business Intelligent Features 

Excel can be used to analyze large set of data with the following features:

- PowerQuery and DAX
- PowerPivot table
- PivotChart

The primary reason to use Excel for business intelligent is because it is a popular software among office workers. However, the main Microsoft software product to perform business intelligent would be the Microsoft PowerBI Desktop.

## Analyzing Daily Peak License Usage

When a quantity of shared software licenses is available for users to check-out and check-in, we need to determine if the current license quantity is sufficient for the user community. Such determination typically will be based on many key indicators and one such key indicators could be the "Daily Peak License Usages".

## Usage Data

The sample data for this analysis is a set of session usages. Each session record has the following attributes:

- UsageLogId
- SoftwareName (APP01)
- LicenseServerName (SERVER01, SERVER02, SERVER03)
- FromDate (check-out time in UTC)
- ToDate (check-in time in UTC)

Note, these data are typically collected and processed from event logs of the license manager software.

There are 3 license servers hosting a total of 11 licenses for application APP01. Each license server has the following number of licenses:

- SERVER01 : 4
- SERVER02 : 3
- SERVER03 : 4

This sample data is available in the file "./Data/AppUsageSessions.zip"

## Using PowerQuery

In this exercise, we will use PowerQuery to calculate the following:

- The daily maximum peak license usage level
- The total time duration when the daily peak reaches the level of maximum available license

Note, the purpose of this exercise is to explore the features of PowerQuery to perform such analysis. The M-code for all the queries is shown in the file [Power Query.txt](./Power%20Query.txt).

## Result

The result of the analysis is displayed as a PowerPivot table and a PivotChart in Excel as shown here:

![Peak License and Duration Chart](./Peak%20License%20and%20Duration%20Chart.png)
