# Superstore-Analysis-2015-2018-
I analyzed sales data of a fictional supermarket with the aim of deriving useful insights as regards the business operation 
Superstore is a Supermarket located in California,United States. They offer a huge variety of goods including but not limited to Books, Art and Appliances. They sell their products on retail and online.
We will attempt to clean the dataset and then carry out analysis on it to derive useful insights. This will be done in Microsoft Excel and then we will prepare a Sales dashboard in Power Bi.
## Tools Used
* Microsoft Power BI
* Microsoft Excel
## The Dataset 
The dataset contains information on 9800 customers. There is more than 20 fields describing consumer behavior. From category of goods to ship mode, this dataset is a rich source of information which contains useful metrics which could give help us identify any trend or patterns in our customers.
## Data Cleaning 
Some of the data cleaning measures I took include:
* Checking for duplicates
* Checking the data type
* Checked the dates field for consistency
* Checked for typos and misspellings
## Data Querying 
1. Total Revenue Generated: To answer this question, the SUM function is used thus:
<br> =SUM(J2:J98011)
<br> which yields $2, 261,536.78 as the result.
2. Lowest Revenue Generated: MIN function was called upon to solve this problem,
<br> =MIN(J2:J9801)
<br> with value $0.44 as the value
3. Total Number of Sales Made: For this part the COUNT function was used to return the result as such:
=COUNT(N2:N9801)
<br> This gives us 9800. This means that a total of 9800 sales were made.
4. Number of Cities where Bussiness is Located: COUNTA function was used here. It was paired with the UNIQUE identifier to pick out distinct values in our dataset.
=COUNTA(UNIQUE(N2:N9801)
<br> This returns 529
5. Determine the Customer responsible for the Highest Sales in the Company: To get the desired output, we used VLOOKUP to get the name of the customer corresponding to the highest Sales made.
=VLOOKUP(X3,G:H,2,FALSE)
<br> which returns Sean Miller as the Highest Paying Customer.
6. Determine the Customer with the Lowest Sales in the Company: We also employ the VLOOKUP function to get this value, the syntax is pretty much the same except we will looking for the name in the Customer Name clumn that corresponds with the lowest sale. The formula is written as:
=VLOOKUP(X4,G:H,2,FALSE)
<br> This returns as Zuschuss Carroll as the answer. Meaning that Zuschuss Carroll has made the lowest purchase yet.
7. What is the Total Revenue generated in “Kentucky”: For this question, we use the SUMIF function. The syntax is :
=SUMIF(L2:L9801,L3,J2:J9801)
<br> Which gives $36,458.39 as the answer.
## Data Visualization 
We loaded the dataset into Microsoft Power Bi. Here I created a dashboard containing key visuals. A dashboards is a great way to display key information about a business. It provides a way to assess the performance of the business. 
<br> I prepared a dashboard showing relevant KPIs such as:
* Revenue
* Number of Orders
* Number of Customers
* Product Count
* Number of Cities in Operation
<br> The visuals used in the dashboard include;
* Sales by Category
* Sales by Subcategory
* Sales by State
* Sales by Region
* Ship modes and their preference by Customers
* Sales by Segment
* Orders and Sales by Year
* Orders and Sales by Month 
