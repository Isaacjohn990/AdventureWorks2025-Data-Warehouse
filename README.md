# AdventureWorks2025-Data-Warehouse

**Database and Schema Setup**

**1. Database Overview**

This project uses Microsoft SQL Server and the AdventureWorks2025 database to build a SQL Data Warehouse using the Medallion Architecture.
The project organizes data processing into three schemas within the same database: Bronze, Silver, and Gold.

**2. Medallion Architecture**

**Layer	        Description**
____________________________________________________________________________________________________________________
**Bronze** -	Stores raw data ingested from the source tables, preserving the original structure as closely as possible.
____________________________________________________________________________________________________________________
**Silver** -	Contains cleaned, validated, and standardized data to improve data quality and consistency.
____________________________________________________________________________________________________________________
**Gold** -	Contains business-ready data organized into fact tables and dimension tables for reporting and analytics.

**3. Schema Creation**

The three schemas are created within the AdventureWorks2025 database using SQL Server's CREATE SCHEMA statement.

USE AdventureWorks2025;
GO

CREATE SCHEMA Bronze;
GO

CREATE SCHEMA Silver;
GO

CREATE SCHEMA Gold;
GO
   
