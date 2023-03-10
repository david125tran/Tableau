# Tableau - Data Visualization  
  
All work done in Tableau (version 2019.2.2).  I did this under the Udemy course, Tableau 2022: A-Z: Hands on Tableau Training for Data Science by Kirill Eremenko. In each section, I attach a file to analyze.  I then attach my Tableau worksheets from the data.  

Section 2 - P1-OfficeSupplies file shows different office supplies, price, and units sold by sales representative (Rep)
1) Most Total Sales Per Region - I show which sales representative (Rep) had the most total sales.  I created a calculated field in Tableau to show who had the most total sales per region.  Total Sales = (Units * Unit Price)

Section 3 - P1-Long-Term-Unemployment-Statistics shows unemployment data 
1) Unemployment vs Month of Period. Grouped by Age.  20 to 24 Year Olds Only - I create an area chart with filters to show amount of unemployed vs. time to show 20 to 24 year olds only.
2) Unemployment vs Month of Period. Grouped by Age.  Men and Women - I create an area chart with filters to show amount of unemployed vs. time to show men and women grouped by age.
3) Unemployment vs Month of Period. Grouped by Age.  Women Only - I create an area chart with filters to show amount of unemployed vs. time to show women only grouped by age.

Section 4 - P1-AmazingMartEU2 file has multiple tables showing orders, sales, region, profit, etc.  
1) Profit Margin and Sales - I do an inner join on the tables ListOfOrders and OrderBreakdown tap into the data source.  
a) Map of Europe Sheet - I made a geographical hierarchy to show country > state > city.  I then filtered by year with the profit margin demonstrated in color (red to blue) and the sum of the sales demonstrated in size.  
b) Customer Scatter Plot Sheet - I show sales vs. profit by customer name which can be filtered by year.  
c) Dashboard w/State Filter - I create an interactive dashboard with an added hover action to show the customer scatter plot by state.  This can be filtered by year.  
d) Dashboard w/Highlighting - I create an interactive dashboard with an added hover action to show the state of the selected customers or show the customer scatter plot by state.  This can be filtered by year.  
2) Sales and Target - I do a data blend of P1-AmazingMartEU2 file to create a dual axis chart which shows sales vs. targeted sales over time.  The dual axis chart has a syncronized axis.  I also create a calculated field which shows the excess of target over time.  
  
Section 5 - P1-Airline-Comparison shows two different airlines with different revenues over different financial quarters.  
1) Airline Comparison - I do a blend of the file to show a comparison of the revenues of the two airlines split up by region.  I do a blend instead of a join because the tables have different levels of granularity for the region.  One airline covers more regions and thus has more granularity.  
  
Section 6 - P1-UK-Bank-Customers  
1) Bank Customers Distribution  
a) Map - I set the Region dimension into a geographical location.  I then configure the unknown locations so that Tableau can understand where they are to show the geographical distribution of the customer base.  
b) Gender - I show the gender distribution of the customer base as a percentage.  
c) Age - I show the age distribution of the customer base in bins.  I create a parameter for the age groups so that the bins can be either 1, 5, or 10 year age bins.  
d) Balance - I show the balance distribution of the customer base in bins.  I create a parameter for the balance groups so that the bins can be any balance that is typed in.  
e) Job - I show the job distribution of the customer base as a tree map.  
f) Customer Segmentation Dashboard - I create an interactive dashboard that shows the map, gender, age, balance, and job distribution of the customer base.  Where you can click on individual dimensions to see how the rest of the customer distribution changes.  
g) Customer Segmentation Storyline - I create an interactive storyline to look at customer distribution across the different countries.  
  
Section 7 - I clean up file P1-PersonalVehicleSalesGlobal_Dirty to make P1-PersonalVehicleSalesGlobal_Cleaned.  I then work with the cleaned file.  
1) Global Vehicle Sales - I use the Tableau data interpreter on the P1-PersonalVehicleSalesGlobal_Cleaned file.  I then perform a pivot on the years & use the metadata grid to rename the pivot column names.   
a) Vehicle Sales - From the modified data source, I then create a visual of the % of total vehicles sold by region.  
b) Global Map - I create a visual of global vehicle sales filtered by year. 
