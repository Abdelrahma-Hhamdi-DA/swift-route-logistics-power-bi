SwiftRoute Logistics | Operations & Performance Analysis
An interactive Power BI project designed to analyze logistics operations, monitor delivery performance, and evaluate the efficiency of hubs, drivers, and vehicles.
Project Overview
SwiftRoute Logistics is an end-to-end data analytics project built to provide a clear view of logistics and delivery operations. The project explores order volumes, on-time delivery performance, customer satisfaction, delivery time, hub capacity, driver performance, and vehicle utilization.

The solution was developed in Microsoft Power BI, using Power Query for data preparation and transformation, and data modeling to connect operational entities and support interactive analysis.

The report is organized into multiple pages, allowing users to move from a high-level operational overview to detailed analysis of hubs, drivers, vehicles, and delivery delays.
Business Objectives
- Monitor overall logistics and delivery performance.
- Track order volume and key service-level indicators.
- Measure on-time delivery rate and customer satisfaction.
- Compare delivery performance across hubs.
- Evaluate hub order volumes against processing capacity.
- Analyze driver experience, performance ratings, and delivery delays.
- Monitor vehicle activity, maintenance status, and order distribution by vehicle model.
- Explore delivery patterns by date, month, year, and operational dimensions.
- Support data-driven decisions to improve operational efficiency and service quality.
Tools & Technologies
Tool / Technology	Purpose
Microsoft Power BI	Interactive dashboards and data visualization
Power Query	Data cleaning, transformation, and preparation
Data Modeling	Connecting operational tables and building the analytical model
DAX	Measures, KPIs, and business calculations
Date Table	Calendar-based analysis and time filtering


Dataset & Data Structure
The project uses logistics-related data organized into the following tables, as shown in the Power BI model:
Table	Description
Orders	Order details, delivery dates, delay reasons, delivery duration, customer satisfaction, and related operational information
Drivers	Driver details, employment type, experience, hire date, and performance rating
Hubs	Hub identifiers, names, and processing capacity
Vehicles	Vehicle identifiers, models, purchase dates, status, and related vehicle attributes
Date Table	Calendar attributes used for time-based analysis
Measure	Dedicated table for organizing measures
Selected Measure	Supports measure selection in interactive report visuals


The model connects operational data to relevant lookup tables to enable analysis across orders, drivers, hubs, vehicles, and dates.
Data Preparation – Power Query
Power Query was used to prepare the source data before building the analytical model.

The preparation workflow included:
- Reviewing the source tables and their columns.
- Promoting the first row to headers where required.
- Assigning appropriate data types to columns.
- Applying locale-aware date and data type transformations where needed.
- Filtering rows and replacing values as part of the cleaning process.
- Preparing the tables for relationships and reporting.
Data Modeling
A relational data model was created in Power BI to connect the main operational tables.

The model includes:
- Orders as the central operational table.
- Drivers, Hubs, and Vehicles as related business entities.
- A dedicated Date Table for calendar-based analysis.
- Supporting tables for measures and dynamic measure selection.
The Date Table contains calendar attributes such as date, day, month, and month number. Relationships between the tables allow report users to analyze operational results by different business dimensions.
Dashboard Pages & Features
1. Logistics Overview
The main dashboard provides a high-level summary of logistics performance through four key KPIs:
KPI	Displayed Value
Total Orders	1,174
On-Time Delivery Rate	78.6%
Customer Satisfaction (CSAT)	82.6%
Average Delivery Time	36.28 hours


The overview also presents:
- Orders processed versus hub capacity.
- Hub performance ranking.
- Driver experience versus performance rating.
- Drivers with the most delivery delays.
- Active versus maintenance vehicles.
- Total orders by vehicle model.
2. Hub Overview
This page focuses on hub capacity and operational performance.

Key visuals include:
- Total orders processed compared with hub capacity.
- Hub performance ranking.
- A weekday heatmap showing hub processing patterns.
- A comparison of processing hours across hubs and days of the week.
3. Drivers Overview
This page evaluates driver performance and delivery activity.

Key features include:
- Total number of drivers.
- Driver experience versus performance rating.
- Drivers with the highest delay percentages.
- A driver selection slicer for individual driver analysis.
- Driver profile details, including hire date, years of experience, and performance rating.
- Monthly trend analysis with a selectable performance measure, including on-time delivery rate.
4. Vehicle Overview
This page analyzes the vehicle fleet and its contribution to delivery operations.

Key features include:
- Total number of vehicles.
- Active versus maintenance vehicle distribution.
- Vehicle age versus breakdown analysis.
- Breakdown count by vehicle model.
- Total orders by vehicle model.
- Breakdown count by vehicle code.
- Orders by vehicle type, such as vans, trucks, pickups, and box trucks.
5. Delay Reason
A dedicated report page is included for delivery delay analysis, accessible through the dashboard navigation.
Interactivity & Filters
The report includes interactive navigation and slicers to help users explore the data.

Available filters shown in the report include:
- Year
- Month
- Vehicle Type
- Vehicle Status
- Driver Name
- Selectable performance measure
Filter availability varies by report page. Users can navigate between the Overview, Hub, Drivers, Vehicle, and Delay Reason pages.
Key Questions the Dashboard Helps Answer
- What proportion of orders are delivered on time?
- How does customer satisfaction compare with delivery performance?
- Which hubs process the highest order volumes relative to their capacity?
- Which drivers have the highest delay percentages?
- How are driver experience and performance ratings related?
- Which vehicles or vehicle models have the most recorded breakdowns?
- How are orders distributed across vehicle types and models?
- How does delivery performance change over time?
These are analytical questions supported by the report's visuals and filters; conclusions should be drawn from the selected reporting period and filter context.
Suggested Repository Structure
SwiftRoute-Logistics-Analysis/
│
├── README.md
├── Dashboard/
│   └── SwiftRoute_Logistics_Dashboard.pbix
├── Data/
│   └── README.md
└── Images/
    ├── logistics-overview.png
    ├── hub-overview.png
    ├── drivers-overview.png
    ├── vehicle-overview.png
    └── data-model.png
Update the filenames to match the files you actually upload. If the original dataset cannot be shared, do not upload private or restricted data; instead, describe the dataset and its availability in Data/README.md.
How to Explore the Project
1. Clone or download this repository.
2. Open the .pbix file using Power BI Desktop.
3. If the source data is not embedded in the report, update the data source paths.
4. Refresh the dataset if required.
5. Navigate through the report pages and use the slicers to explore operational performance.
Skills Demonstrated
- Data cleaning and transformation with Power Query
- Data type and locale management
- Relational data modeling
- Date table creation and time-based analysis
- DAX measures and KPI development
- Interactive report design in Power BI
- Logistics and operational performance analysis
- Hub capacity and utilization analysis
- Driver performance analysis
- Fleet and vehicle performance monitoring
- Business-focused data storytelling
Author
Abdelrahman Hamdi
Aspiring Data Analyst
This project demonstrates the use of business intelligence tools to transform logistics data into an interactive performance monitoring and analysis solution.
