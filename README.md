# Synapse Scalability Simulator
Demos of Synapse Scalability features: Resultset Cache and Materialized Views

![summary](https://github.com/stevemoss-microsoft/SynapseScalabilitySimulator/blob/main/images/Scalability%201.jpg?raw=true)


1) Download SQL Query Stress from Microsoft Store
https://www.microsoft.com/en-us/p/sqlquerystress/9n46qj5sbgkb?activetab=pivot:overviewtab



There are mainly 2 notebooks created to perform profiling and constraint validation separately:

<b>Data Quality Accelerator,</b> notebook gets the profile information. This notebook also get additional information for numeric data e.g. min, max, mean, stdDev etc. as part of the output. Along with profile information, it also helps to identify the constraints which can be applied to your dataset to improve the quality of data and ensure consistency and reliability. It runs the profile in one pass on your specified dataset and does not repeat for efficient operation.

<b>Data Quality Validator,</b> notebook performs validation on your dataset columns against defined constraints. It reports the constraints status along with message which shows unsupported value found in a column which is failed to validate.

## Pre-requisites
1) Requires adding both deequ spark jar, and pydeequ librarys to Databricks cluster. You can find the library to install in lib folder of this repository
[how to add a library to a databricks cluster](https://docs.microsoft.com/en-us/azure/databricks/libraries/cluster-libraries)


