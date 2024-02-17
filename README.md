
# Project Title

A brief description of what this project does and who it's for

# Axon sales-Dashboard

### Dashboard Link : https://app.powerbi.com/view?r=eyJrIjoiZjhmNGEyNmYtYzMxMC00ZWE4LWEwYjktMTQ4OTg3Mjk2ZmI4IiwidCI6IjQ4MmQzMTQzLTYzMGUtNDI0My05YmQzLTdhYjZhNzdjYWY5ZCJ9

## Problem Statement

A small company Axon, which is a retailer selling classic cars, is facing issues in managing and analyzing their sales data. The sales team is struggling to make sense of the data and they do not have a centralized system to manage and analyze the data. The management is unable to get accurate and up-to-date sales reports, which is affecting the decision-making process.

This dashboard helps the Axon company understand their business better. It helps company to know their total sales,how much profit they are generating who are their Top customer, their Top Products,they got information about their sales representative.


Since they has largest sales market in USA and lowest customer are from singapore they has to do more focus on singapore market.
### Steps followed 

- Step 1 : Import and integrate the data from MySQL database into PowerBI
- Step 2 : Open power query editor & in view tab under Data preview section, check "column distribution", "column quality" & "column profile" options.
- Step 3 : Also since by default, profile will be opened only for 1000 rows so you need to select "column profiling based on entire dataset".
- Step 4 : It was observed that in customers table there was some null values,so replaced null values.Employee table has some duplicates values ,so removed duplicates. 
- Step 5 : For calculating sales price,profit and cost price we created calculated columns
- step 6 : we created a date table using calenderauto() function:
- Step 7 : In the report view, under the view tab, theme was selected.
- Step 8 : We created 3 page dashboard contaning sales,products and sales representatives information respectively.
- Step 9 : Visual filters (Slicers) were added for year and monthly sales.
- Step 10 : card visuals were added to the canvas, one representing Total Sales,Total profit ,total Orders ,total customers& total orders .

- Step 11 : Bar chart was also added to the sales report design area representing the sales according to Products, productlines and customer name. Pie chart added to sales report for total salesby country.

- Step 12 : In the report view, under the insert tab, using shapes option from elements group a rectangle was inserted for title of the dashboard. 

        
- Step 13 : New measure was created to find total Sales.
Following DAX expression was written for the same,
        
        Total sales = sum(sales price)
        
A card visual was used to represent count of customers.
![Screenshot 2024-02-17 161659](https://github.com/syedayeshakhan/Axon_Sales_powerBI/assets/159778073/8916b1dd-1060-4c83-95da-68b6c6c81383)




        
 - Step 16 : New measure was created to find  Profit Margin ,
 
 Following DAX expression was written to find % of customers,
 
         Profit Margin % = [total Profit]/[total Sales]
 
 A card visual was used to represent this perecntage.
 
 Snap of % of Profit Margin
 
 ![Screenshot 2024-02-17 162551](https://github.com/syedayeshakhan/Axon_Sales_powerBI/assets/159778073/25509a07-6e10-4969-8d2e-d57f5db2d0c1))

 
 - Step 17 : New measure was created to calculate total profit
 
 Following DAX expression was written to find total profit,
 
         Total Profit= sum(sales)-sum(cost price)
    
 A card visual was used to represent this total Profit,
 
 

![Screenshot 2024-02-17 164005](https://github.com/syedayeshakhan/Axon_Sales_powerBI/assets/159778073/34f30381-618e-4489-8ad3-86306556f891)

 

 - Step 18: Created  1 introduction page and 3 sales report pages,
 - page 1 Sales Pae :Dashboard containing diffrent visuals as bar chart,column chart for analyzing sales using top 5 prodcut,Top 5 productline,sales by Top 5customers,used a pie chart for country wise sales used a line chart for yearly and monthly sales.


 - Step 19 : The report was then published to Power BI Service.
 #
 #
 ###
 
 ![Screenshot 2024-02-17 165554](https://github.com/syedayeshakhan/Axon_Sales_powerBI/assets/159778073/58f79f18-e148-4197-ac7b-fa7d08cf61b0)



 #


 #
 # Snapshot of Dashboard Page 1 (Power BI Service)

![Screenshot 2024-02-17 170800](https://github.com/syedayeshakhan/Axon_Sales_powerBI/assets/159778073/8d88d753-289f-4f8d-b920-185d600a8014)

#
#
- Page 2 Products:

# Snapshot of Dashboard (Power BI Service)




![Screenshot 2024-02-17 171317](https://github.com/syedayeshakhan/Axon_Sales_powerBI/assets/159778073/6d0182cf-6ee9-40ae-b151-beec833443f0)




- Page 3 Sales Representative:
 # Report Snapshot (Power BI DESKTOP)



 ![Screenshot 2024-02-17 171620](https://github.com/syedayeshakhan/Axon_Sales_powerBI/assets/159778073/36f35e29-c64c-402f-9142-9804563c1098)

# Insights


3 Pages Dashboard created on Power BI Desktop & it was then published to Power BI Service.

Following inferences can be drawn from the dashboard;

### [1] Top 5 Customers By sales are:

   
[1] Euro + Shopping Channel

[2] Mini Gifts Distributors
   
[3] Australian Collectors Co.

[4] Muscle Machine inc.

[5] La Rochelle Gifts


        
           
### [2] Top 5 Products are:

[1] 1992 Ferrari 360 Spider red

[2] 2001 Ferrari Enzo

[3] 1952 Alpine Renault 1300

[4] 2003 Harley-Davidson Eagle Drag Bike

[5] 1968 Ford Mustang




  ### [3] Top 5 Country by Sales:
  
[1] USA

[2] Spain

[3] France

[4] Australia

[5] New Zeeland

#

 ### [4] Top 5 Productlines by Totalsales
 
[1] Classic Cars

[2] Vintage Cars

[3] Motorcycles

[4] Trucks and Buses

[5] Palnes
 

         
### 
       
       Thus we have top sale from "USA" and top Most Selling product is  "992 Ferrari 360 Spider red" 
       highest sales are from "Classic Cars" Category.

### 

- Lowest sales product :



        "1939 Cheverolet Delux Coupe" has lowest sale and very less orders are from "Trains"
         Category and very less orders recieved from " singapore"
