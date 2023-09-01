# Energy_consumption_report
Power bi based Energy Consumption report to show the different form of energy used by a company in different buildings in USA.
https://github.com/rajni-kapoor/Energy_consumption_report/edit/main/README.md
Energy Consumption Report <br>
https://github.com/rajni-kapoor/Energy_consumption_report/blob/main/utilities-save-natural-resources-vector-set-of-images-of-electricity-gas-and-water-2GCRJYY.jpg
About the project: In this project I will analyze the data regarding the energy consumption of a company in various form like electricity, gas and water in USA. This analytic project will help the management to take data-driven decisions to track the consumption and cost of different energy sources. <br>


Data set: Excel work sheet <br>
## Problem-Statement:  
The company has faced financial crisis because of excessive energy consumption, and asked to analyze the data and provide insights so that management can take decision to improve the energy consumption. There are three tables Energy consumption, rates and Building master.

![image](https://github.com/rajni-kapoor/Energy_consumption_report/assets/123319398/aa3973f9-da52-4347-92aa-6acebbb69022)



# Data Cleaning and Transformation:  
  The data was in a excel format which I import in a power bi desktop application and used power query editor to scrub the data. Following were the steps I took:<br>
•	Used first row as headers in Building master <br>
•	Remove Duplicate records <br>
•	In energy consumption table, I will transform columns Water consumption, Gas consumption and Electricity consumption into one column Consumption_type using unpivot.<br>
•	Using replace values option I will remove consumption from the Consumption_type column’s values.<br> 
•	In rates table, I will create a key column by merging year and Energy type.<br>
•	In Energy Consumption table, I will extract the year from the date and then create a column key by merging year with Consumption_type. <br>
•	In the data model tab, the relationship is automatically detected among the three tables with the help of common column Building and Key. <br>
•	I created DAX measure Total Cost and Unit Consumed. <br>
 
Relationship modeling: <br>
![image](https://github.com/rajni-kapoor/Energy_consumption_report/assets/123319398/e5779f90-cf0d-41aa-86dc-0735b3e17ff1)


# Dashboard design : 
• The energy consumption report is 4 page report where the main page gives the overview of the report. <br>
• I used the card to show the Total cost and Unit consumed by the company which can be modified by selecting values using slicers of consumption_type, building, city and date range. <br>
• Donut chart shows the unit consumed by Water, Electricity and Gas. The maximum amount of unit is consumed by Water at approximately 88%, while gas has consumed only 2% unit. <br>
• The map chart shows the various location of company’s building in USA. The bubble size is demonstrated with the help of Total cost. <br>
• The tree-map shows the all buildings and their volume is showed by the unit consumed by the respective building. <br>
• Total cost and consumption type used the stacked column chart and Date in x-axis throughout the given period. <br>
• Similarly I made 3 more pages for the dedicated energy sources to show the data related to that energy. All the pages are connected using page navigator button. <br>
• I also generated a short summary with the help of smart narratives. <br>
• I used conditional formatting to show the data bars for Unit Consumed and Tota Cost in the table. <br>
• I used waterfall chart to show the increment of the total cost in all cities. <br>

Main report:<br>
![image](https://github.com/rajni-kapoor/Energy_consumption_report/assets/123319398/309d0b85-dc71-481b-bcbb-d358dfb2af21)



Water consumption : <br>

![image](https://github.com/rajni-kapoor/Energy_consumption_report/assets/123319398/2e53de96-9896-4896-afe7-d6bc8230df63)


Electricity consumption:<br>

![image](https://github.com/rajni-kapoor/Energy_consumption_report/assets/123319398/1cb409fa-0bd5-4e59-b593-0ef96978acf3)

Gas consumption: <br>

![image](https://github.com/rajni-kapoor/Energy_consumption_report/assets/123319398/5a09e91f-a2b2-454a-be53-6a5fe23903c1)






