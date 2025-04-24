### SQL with Azure Databricks Lab
This lab provides a hands-on introduction to using SQL in Azure Databricks. You'll learn how to create a SQL Warehouse, define databases and tables using Delta Lake, and visualize data with dashboards—all within the Databricks environment.

### Prerequisites
An active Azure subscription with sufficient quota

Admin access to the subscription

PowerShell environment in Azure Cloud Shell

### What You'll Do
Provision Azure Databricks Workspace using a setup script

Start and configure a SQL Warehouse

Create a database schema and table from a CSV file

Query data using SQL

Build and publish a dashboard

### Setup Instructions
Open Azure Cloud Shell in PowerShell mode and run:

rm -r mslearn-databricks -f
git clone https://github.com/MicrosoftLearning/mslearn-databricks
cd mslearn-databricks
./setup.ps1

ℹ️ The script provisions a Premium-tier Azure Databricks workspace in a region with available compute quota.

### Dashboard Example
Create a bar chart that displays product categories and their count using the retail_db.products table.

SELECT ProductID, ProductName, Category FROM retail_db.products;

### Clean Up
After finishing, stop your SQL Warehouse in the Databricks portal to avoid extra costs.

