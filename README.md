# HR_Analytic_Project
Power BI
## Objective 
An HR person wants to know the overall presence percentage of employees in the office. 

## Dataset
<a href = "https://github.com/rinasingh1/HR_Analytic_Project/blob/main/Attendance%20Sheet.xlsx"> View HR analytic Project</a> This project is based on the count of 189 data points. 

## Data Cleaning and processing
<br>

How to combine different sheets having different columns into a single sheet. 

•	Bring all the sheets together to transform in the power query editor.
<br>

•	Duplicate the Worksheet (an original Worksheet named Attendance Sheet) while giving it a different name in the power query editor for example – “template”
<br>

•	Out of 3 sheets in the worksheet the one sheet named “April 2022” has been selected. 
<br>

•	Here an option comes ‘Change data type’ in the Applied Steps section needs to be deleted, as, if we don’t delete the column type of this sheet, it will be referenced by other sheets having different columns.
<br>

•	A parameter is created so that through this parameter we can reflect the rule of one sheet in other sheets as well. For example –  parameter name here is “Worksheet”.
<br>

Data cleaning 
<br>
•	Promoting top row as headers 
<br>
•	Removing top rows
<br>
•	Determining data type of all columns 
<br>
•	Removing errors
<br>
•	Unpivoting some columns

## Calculated Columns 
using DAX 4 calculated columns are added to the table 
<br>

•	WFH Count – SWITCH()
<br>

•	SL Count -  SWITCH()
<br>

•	Day of Week – Formatting function is used
<br>

•	Month – STARTOFMONTH ()


## Measures 
A measure table is created to keep all the measures in one place.
<br> 

using DAX the following measures are created 
<br>

•	Total Working Days – using VAR and CALCULATE()
<br>

•	Present Days – using VAR and CALCULATE()
<br>

•	Present % - DIVIDE()
<br>


•	WFH Count – SUM()
<br> 

•	WFH % - DIVIDE()
<br>

•	SL Count – SUM()
<br>

•	SL % - DIVIDE()

## Project Insights 
•	The total presence percentage in the office  is 91.83% and it is decreasing. 
<br>


•	Tuesday is the day when most of the employees are present i.e, 93%.
<br>


•	WFH (Working From Home) percentage is increasing and it is high on weekends i.e Friday.
<br>



•	SL (Sick Leave) percentage is increasing, it is lowest in April, while it is increasing moving ahead e.g June. On regular basis it is high on Monday i.e, 1.62%.
<br>



•	Two tables are provided through which we can analyse the presence percentage of an individual employee. The Highest present %, The lowest present %


## Conclusion 
On the basis of the presence percentage in the office showing a decrease in the future, we can plan accordingly to optimise this trend. We can consider directing some percentage work from home. The free space can be lent out to rent and there would be a decrease in the cost of electricity, water supply and maintenance. We can use Tuesday to arrange some team building activity like team lunch. 
Sick leave percentage is increasing, like in this dataset May is the month having highest sick leave percentage, the reason behind it may be the seasonal change from spring to summer causing increase in temperature, humidity and spread of allergens. So it is important to know the reason behind it, so that we can take measures accordingly. 










