# SynapseScalabilitySimulator
demos of Synapse Scalability features

1) Download SQL Query Stress from Microsoft Store
https://www.microsoft.com/en-us/p/sqlquerystress/9n46qj5sbgkb?activetab=pivot:overviewtab


# DataQ Accelerator
Easily Implemented Big Data Profiling And Data Quality Tool

DataQ accelerator is a notebook based solution to perform data profiling, constraints suggestions and constraints validations on data stored in Azure Data Lake Store Gen2. DataQ accelerator works well with CSV and Parquet file format to perform data quality operations and validations. 

DataQ notebook implements and automates an open source Deequ library. It is spark library under Apache 2.0 license developed by Amazon AWS.

![summary](https://github.com/stevemoss-microsoft/
SynapseScalabilitySimulator/blob/main/images/Scalability 1.jpg?raw=true)

There are mainly 2 notebooks created to perform profiling and constraint validation separately:

<b>Data Quality Accelerator,</b> notebook gets the profile information. This notebook also get additional information for numeric data e.g. min, max, mean, stdDev etc. as part of the output. Along with profile information, it also helps to identify the constraints which can be applied to your dataset to improve the quality of data and ensure consistency and reliability. It runs the profile in one pass on your specified dataset and does not repeat for efficient operation.

<b>Data Quality Validator,</b> notebook performs validation on your dataset columns against defined constraints. It reports the constraints status along with message which shows unsupported value found in a column which is failed to validate.

## Pre-requisites
1) Requires adding both deequ spark jar, and pydeequ librarys to Databricks cluster. You can find the library to install in lib folder of this repository
[how to add a library to a databricks cluster](https://docs.microsoft.com/en-us/azure/databricks/libraries/cluster-libraries)


