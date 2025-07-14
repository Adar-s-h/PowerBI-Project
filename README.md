# PowerBI-Project

OBJECTIVE 
 
The primary goal of this project is to analyze customer churn trends and identify actionable 
insights that businesses can use to retain more customers. The specific objectives include: 
• Analyze Overall Churn Trends: Evaluate the overall churn rate and observe how it changes 
across various customer segments. 
• Understand Demographic Factors: Examine how gender, age, senior citizenship, and family 
status affect customer retention. 
• Explore Financial Influences: Determine the role of monthly charges, payment method, and 
total spend in influencing customer behavior. 
• Assess Impact of Tenure: Investigate if shorter customer tenure correlates with higher 
churn risk. 
• Examine Contract Types: Compare churn rates across monthly, one-year, and two-year 
contract customers. 
• Visualize Key Metrics: Build a comprehensive dashboard to present KPIs such as total 
customers, churned customers, retention rate, and average monthly billing. 
• Enable Strategic Planning: Equip management and customer success teams with data
driven insights to guide retention campaigns. 
• Support Interactive Decision-Making: Utilize Power BI’s interactivity (slicers, filters, 
tooltips) to allow dynamic exploration of customer data.

METHODOLOGY & DATA ANALYSIS 
 
 
The methodology for this project follows a structured, step-by-step process starting from data 
acquisition to the creation of an interactive Power BI dashboard. The aim was to transform raw 
customer data into meaningful business intelligence that aids in decision-making. The steps below 
outline the full analytical pipeline: 
 
Step 1: Data Importation 
The dataset was imported into Power BI Desktop using the Power Query Editor. The original file 
was in a structured CSV format containing over 7,000 records and more than 20 fields. These 
fields included customer demographics, contract details, billing amounts, and a churn indicator. 
 
Step 2: Data Cleaning 
Before analysis, the dataset underwent rigorous cleaning: 
• Missing Values: Columns were checked for null or blank entries, especially in critical fields 
like tenure, total charges, and churn status. Appropriate imputation or row removal was 
applied. 
• Data Types: Numeric fields (e.g., tenure, monthly charges) were converted to proper data 
types. Binary and categorical fields (e.g., gender, contract type) were standardized. 
• Formatting: Text fields were cleaned for consistency (e.g., correcting capitalization issues, 
standardizing “Yes” and “No” responses). 
 
 Step 3: Feature Engineering 
Several calculated columns and DAX measures were added: 
• Churn Rate (%) = (Churned Customers / Total Customers) × 100 
• Active Customers = COUNT of customers where Churn = "No" 
• Tenure Buckets = Custom bins: “0–12 months”, “13–24 months”, “25+ months” 
• Revenue Risk = SUM of monthly charges for churned customers 
 

Step 4: Data Modeling 
A star schema was created where necessary, ensuring dimension fields like gender, payment 
method, and contract type were properly linked to the main customer fact table. Relationships 
were verified to support accurate slicing and filtering in visuals. 
Step 5: Dashboard Construction 
Key dashboards were designed with the following elements: 
• KPI tiles for total customers, churned count, average tenure, and average monthly charges. 
• Interactive charts to show trends and comparisons across demographics and 
contract/payment types. 
• Slicers and filters for gender, senior citizen status, and contract length to enhance 
interactivity. 
• Drill-through pages for customer-level exploration. 
The methodology ensured the integrity of analysis and a visually compelling user experience.

RESULTS & VISUALIZATION 
 
The Power BI dashboard produced from this project offers a comprehensive, visual 
representation of customer churn behavior. Below are the main visualization components 
and the insights they provide: 
KPI Cards 
• Total Customers: Displays the total number of customers in the dataset. 
• Churned Customers: The count of customers who have left the company. 
• Churn Rate (%): A quick metric for understanding the overall attrition rate. 
• Average Tenure: Indicates how long, on average, customers stay before they churn. 
• Average Monthly Charges: Provides a view of the revenue scale and its relation to churn. 
Donut and Pie Charts 
• Churn by Contract Type: Highlights that customers on month-to-month contracts have 
significantly higher churn rates compared to those on annual or two-year contracts. 
• Churn by Payment Method: Shows that customers using electronic check payment are 
more likely to churn than those using bank or credit card auto-payments. 
Bar Charts 
• Tenure vs Churn: Bar chart segments customers by tenure buckets, confirming that newer 
customers (0–12 months) have the highest churn risk. 
• Monthly Charges vs Churn: Reveals a trend where customers with higher monthly 
charges are more likely to leave, possibly due to perceived lower value for cost. 
Treemap 
• Churn by Internet Services: Identifies which services (e.g., streaming TV, online security) 
are linked to higher churn, helping prioritize service improvements. 
Segmented Analysis 
• Churn by Senior Citizen: Shows senior citizens slightly more likely to churn. 
• Churn by Gender and Dependents: Offers gender-based and family status insights. 
 
Slicers & Tooltips 
Interactive slicers allow users to filter by demographic fields or service usage. Custom tooltips reveal      
detailed metrics on hover, such as total charges and contract tenure of churned users. 
These visual elements not only make the report easy to interpret but also encourage business users to    
interact with the data and derive their own insights.

<img width="1442" height="810" alt="Churn Dashboard  - PowerBI" src="https://github.com/user-attachments/assets/dcd6e97c-d9eb-4962-bf88-4dfdf81df6f5" />
