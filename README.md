# Power-BI-Assignment-Data-Transformation-Data-Modeling-1
E-Commerce Sales Analysis
Data Transformation:
●	Restrict the "List of Orders" table to only the first 500 rows by the transform to power query then select the coloumn of list of orders then go to home -keep rows-keep top rows -rows enter 500 then ok the rows will be reduced to 500.
●	Ensure the “Order Date” column in the “List of Orders” table is set to data type 'Date'-select the order date coloum in power query then go to home-data type date then select date.
●	Format	the	"CustomerName"	column	into	proper	case,	ensuring consistent capitalization for each word-select the column of customer name then select transform-then click format then capitalize each word and also done trim and clean .
●	Merge the "State" and "City" columns to create a new column named "Location" in the format ‘City, State’-first add a column - select both state and city columns then go to transform -merge coloumns from ribbon then seperated by comma and give column name as 'Location'.
●	Create a new custom column named "Profit Margin" as the percentage of "Profit" divided by "Amount".create a new column using add coloumn then select add custom column using this syntax create a column named Profit margin if [Amount] = null or [Amount] = 0 or [Profit] = null then null else [Profit] / [Amount] then it is converted to decimal data then close and apply .then the profit margin coloumn selected in power BI then click column tools then select format from ribbon then click percentage .
●	Add a new conditional column named "Profit Status" based on the values in the "Profit" column. The conditions are as follows: if the profit is less than 0, the label should be "Loss"; if the profit equals 0, the label should be "Break-Even"; and if the profit is greater than 0, the label should be "Profit"-add coloumn named profit status and use this syntax if [Profit] = null then "Unknown"else if [Profit] < 0 then "Loss"else if [Profit] = 0 then "Break-Even" else "Profit".
Merging Data (Joins):
●	Merge the "List of Orders" and "Order Details" tables into a new single table named "Orders Data" based on the "Order ID" relationship-select table named list of orders then go to home and select merge queries from tab -select merge queries as new then select both tables that we need to merge then slect order id coloumn in both table then give a join kind like left outer which means all from first and matching from second table then click ok then rename the new table as orders data.
Handling Missing Data & Duplicate Data:
●	Identify missing values in the data and determine a strategy to address them-

