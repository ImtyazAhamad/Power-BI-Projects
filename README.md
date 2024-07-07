# Sales Dashboard (Customers/Products)

### Dashboard Link : 
https://app.powerbi.com/groups/me/reports/271f3001-eb7c-4492-b154-15e5333e7df4/b5b69f3da40209bc5361?experience=power-bi

### Problem Statement

The business request for data analyst project was an executive sales report. 
Based on the request that was made from the business, we following user stories were defined to fulfill delivery and ensure that 
acceptance criteria’s were maintained throughout the project.

## Business requirements 
     1-	To get a dashboard overview of sales as per customers and products.
     2-	Dashboard which allows me to filter data for each Product
     3-	Dashboard with graphs and KPIs comparing against budget
     4-	Dashboard which allows me to filter data for each customer
     5-	Detailed overview of Sales as per product category

### Steps followed 

- Step 1 : Load data into SQL Server and clean the data.

  ## Following are the code for cleaning of data.


  
- Step 2 : Load the cleaned data into the power BI
- Step 3 : Open power query editor & in view tab under Data preview section, check "column distribution", "column quality" & "column profile" options.
- Step 4 : Made necessary changes such as data types, merging tables, and add calculated columns to make required dashboard.
- Step 5 : Made connection among the table which is crucial for accurate data analysis and visualization.

## Relationship of tables are as follow-

	#Customers to Sales:
	   Type: Many-to-one (*:1)
	   Columns: Customers.Customerkey to Sales.Customerkey
	   Cross Filter Direction: Single

	#Product to Sales:
	   Type: Many-to-one (*:1)
	   Columns: Product.Productkey to Sales.Productkey
	   Cross Filter Direction: Single

	#Calendar to Sales:
	   Type: Many-to-one (*:1)
	   Columns: Calendar.datekey to Sales.Orderdatekey
	   Cross Filter Direction: Single

	#Calendar to Budget:
	   Type: One-to-One (1:1)
	   Columns: Calendar.Date to Budget.Date
	   Cross Filter Direction: Both
 
  ## Data Model
	Below is a screenshot of the data model after cleansed and prepared tables were read into Power BI.
	This data model also shows the connection of tables.
![Data_Model](https://github.com/ImtyazAhamad/Power-BI-Projects/assets/120785398/7b91c2c0-11a4-4b1d-ac1f-2a5bf172f0a7)

## Sales Management Dashboard as per customers
![Sales Overview(Customer)](https://github.com/ImtyazAhamad/Power-BI-Projects/assets/120785398/3a36d580-6b62-491f-9bb0-21337d9d94a4)

## Sales Management Dashboard as per products
![Sales Overview (Product)](https://github.com/ImtyazAhamad/Power-BI-Projects/assets/120785398/28211881-0587-44a5-bbfb-c5e1f8edd0d3)
