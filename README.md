# EXCEL-MODULE-END
<B>CUSTOMER  TABLE</B>
•	United states of  america is replace with --USA
•	Customer name is converted into capital letter also prefix Corrected
•	Missing values in loyalty
•	Customer id has some corrections-- c-1485 to CUST-4521
•	5 duplicate values are present
•	Using COUNTA Function to count total number of customers
         COUNTA(B2:B501)<BR><BR>
PRODUCT TABLE
•	Correction in p-3 to PROD 3
•	Correction in missing values in stock and cost  
•	 Missing values in stock is corrected by using statistical method  mean
•	Cost data type is converted to currency
•	Find total cost using Sum function
•	Subcategory removed
•	Using SUMIF Function to find total cost of “clothing”
SUMIF(Table2[Category],"clothing",Table2[Cost])<BR><BR>


Descriptive statistics
Stock	
		
Mean	268.95	
Standard Error	13.15155155	
Median	273	
Mode	273	
Standard Deviation	131.5155155	
Sample Variance	17296.33081	
Kurtosis	-1.09075743	
Skewness	-0.020492295	
Range	496	
Minimum	0	
Maximum	496	
Sum	26895	
Count	100	
<BR><BR>

SALES TABLE
•	Total Amount missing value is replaced by using this formula
       Total Amount = Quantity*Unit Price/(1 -Discount)

•	Find Performance
         IF(totalamount>3500,"excelnt","good")

•	Discount = 1 -(Total Amount/(Quantity*Unit Price))
•	9 duplicate value
•	Highest price in unit price is highlighted by using
•	data bars
•	Top 10 highest discount is highlighted by using conditional formatting

•	Total Amount column data type is changed
•	Year is extracted from order_date by using TEXT Keyword
        =TEXT([@[Order_Year]],"YYYY")
•	This year used for creating dashboard
•	Using vlookup find performance of store 7
          =VLOOKUP(E13,E1:L91,8)

<UL>DASHBOARD</UL>
•	Summary Cards:
o	Total Customers: 500
o	Number of Store: 20
o	Total Sales: 2174394
•	Charts & Visualizations:
o	Top Sales (Sales Ranking): A bar chart illustrating top stores such as STORE12 (value 5), STORE17 (value 3), STORE3 (value 2), STORE4 (value 4), and STORE8 (value 1).
o	Stock (Sum of Total Stock): A doughnut chart breaking down stock by category: Beauty (4816), Clothing (4931), Electronics (5314), Home (4794), and Sports (7040).
o	Loyalty Level (Count of Customer): A column chart displaying customer counts across tiers: Bronze (125), Gold (122), Platinum (145), and Silver (104).
o	Top 10 Product (Sum of Total_Amount): A horizontal bar chart displaying product sales values, including PROD20 (16605.5037), PROD34 (17694.2172), PROD42 (19770.5232), PROD43 (15772.6566), PROD62 (15922.0094), PROD76 (19714.534), PROD80 (14216.9484), PROD91 (14338.7606), PROD94 (14655.8799), and PROD98 (13960.7317).
o	We can easily find out net profit
o	The donut chart represent payment type that help highest customer prefer which type




