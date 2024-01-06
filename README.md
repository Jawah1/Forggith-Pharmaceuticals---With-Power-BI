# Forggith-Pharmaceuticals-With-Power-BI
Forggith Pharmaceuticals is a Pharmaceutical Manufacturing company based in Germany. As a Manufacturing company, they produce medical drugs that get to the consumers through their Distributors.

In their efforts to maximize growth, Forggith works with a team of Sales and Marketing pros who ensure retailers can get their products through the distributors.

Forggith is looking to create some Power BI Reports to assist in guiding their strategies, tactics, and operations as a company. They have identified a couple of numbers they would like to report from their data as reports.

## Sales Performance Overview (Sliced by: Year, Month, Quarter, Team)

Total Revenue
Total Revenue Year To Date (YTD)
Total Revenue Previous Year YTD
Total Revenue Same Period Last Year(SPLY)
Total Target
Total TargetYTD
Actual Revenue Performance YTD vs Target YTD
Revenue Month-on-Month Percentage Change
Revenue Distribution by Location
Revenue by Channel
Revenue by Product Class

## Marketing Performance (Slice by Year, Quarter, Month, Product Category and Team)

Revenue Achieved vs Revenue Target
Volume Achieved vs Volume Target
Actual Revenue by Sales Representative
Target Revenue Achievement% by Sales Representative
Actual Volume by Sales Representative
Target Volume Achievement by Sales Representative
Actual Revenue Achievement by Sales Team.
Data Structure

## The dataset consists of 8 tables that include information on sales transactions as well as set targets for each year.

DimLocation table: contains the city where the store is located, latitude, longitude, and a unique identifier.
DimChannel table: contains a channel for drug distribution and a unique identifier.
Dim SubChannel table: contains sub-channel for drug distribution, channel ID, and a unique identifier.
DimProducts table: contains price, name, drug class, and a unique identifier.
DimEmployees table: contains the sales rep name, manager, team, and a unique identifier.
Sales2022: contains monthly transactions of products and quantities sold at different stores for 2022.
Sales2023–2025: contains monthly transactions of products and quantities sold at different stores for the years 2023–2025.
Target data: contains set targets for the years 2022- 2025.
Data Cleaning & Transformation

## All eight tables were imported into the Power BI Desktop and transformed into a power query.

Both sales tables had similar column names so they were appended together.
Each dimension table had its unique identifier in the sales table, except the DimChannel table. The DimChannel tabe was joined with the DimSubChannel table using its unique identifier to enable a star schema model.


![Join Dim channel](https://github.com/MohamedAlimamyJawah/Forggith-Pharmaceuticals---With-Power-BI/assets/131864852/1a141f0e-8702-49dc-ad52-d0f44615b9c2)

## Unpivoting columns in the target table


![Screenshot (29)](https://github.com/MohamedAlimamyJawah/Forggith-Pharmaceuticals---With-Power-BI/assets/131864852/e6c4b639-36e0-4721-b8a5-4516e99cbf06)


# Data Modelling

Unique identifiers- Primary keys in the dimension tables were related to the respective columns - foreign keys in the facts tables (sales and target tables).


![Screenshot (30)](https://github.com/MohamedAlimamyJawah/Forggith-Pharmaceuticals---With-Power-BI/assets/131864852/3cec1608-93c8-4dbc-9705-1dce32e78e66)


# Report Building and Visualization


Kep Performace indicator

![B KPI](https://github.com/MohamedAlimamyJawah/Forggith-Pharmaceuticals---With-Power-BI/assets/131864852/8b949d7d-22c8-4033-a4f7-c004f24942c7)


Revenu month on month

![Month on month](https://github.com/MohamedAlimamyJawah/Forggith-Pharmaceuticals---With-Power-BI/assets/131864852/0a4e1b69-0bef-48e8-9a9a-055891db7640)


Revenue by product class

![Total Revenue by product class](https://github.com/MohamedAlimamyJawah/Forggith-Pharmaceuticals---With-Power-BI/assets/131864852/5ae6b12f-3299-4be0-8945-f1b8eaa1fec5)


Revenue by channel

![Revenue by channel](https://github.com/MohamedAlimamyJawah/Forggith-Pharmaceuticals---With-Power-BI/assets/131864852/0f722852-a993-4d6d-8745-994e669d8f3b)


Sales Performance by Cities

![Screenshot (31)](https://github.com/MohamedAlimamyJawah/Forggith-Pharmaceuticals---With-Power-BI/assets/131864852/dd2c225e-4ef4-4673-957e-d4877926b59a)


# Dashboard
![B Dashboard](https://github.com/MohamedAlimamyJawah/Forggith-Pharmaceuticals---With-Power-BI/assets/131864852/997f10b9-1a8d-4f96-87f2-18013ff56f43)


