## EFFICIENCY ANALYSIS FOR AN AUTOMOBILE BRAND

***TABLE OF CONTENTS***

- ***[ EXECUTIVE SUMMARY]( EXECUTIVE-SUMMARY)***
- ***[DATA SOURCES](DATA-SOURCES)***
- ***[BUSINESS PROBLEM](BUSINESS-PROBLEM)***
- ***[METHODOLOGY](METHODOLOGY)***
- ***[SKILLS](SKILLS)***
- ***[THE ANALYSIS CODES](THE-ANALYSIS-CODES)***
- ***[KEY FINDINGS](KEY-FINDINGS)***
- ***[BUSINESS RECOMMENDATIONS](BUSINESS-RECOMMENDATIONS)***
- ***[NEXT STEP](NEXT-STEP)***

  ![Ferrari Car](https://github.com/user-attachments/assets/95ca7dbf-57f0-4900-900c-024a3e56eaad)
---


***EXECUTIVE SUMMARY***

*This analysis aim to provide us with insights on Fuel_types efficiency of the Automobile_Brand, by simple analysing various components
and features to identify trends and purchases to be able to advice the Brand on how to make inform decision about their vehicles to 
increases sales or drive more patronage from customers who want to save cost on Fuel_Consumption and this way the Brand can maximise 
Market opportunities and become a goto source for efficient vehicles that meet their customers needs.*



***DATA SOURCES***

*Automobile Dataset: The Automobile dataset used for this analysis is an excel file which provides us with enough detailed features 
needed to conduct a proper analysis to track vehicle performance and efficiency.* 


***BUSINESS PROBLEM:***

*Vehicle_Efficiency is very important for this AutoMobile Brand in other to be more competitive in the Market and drive sells of their Vehicle to 
customers satisfaction and The Manufacturers wanted to know the following*

*1.) Better ways to improve their Vehicle Efficiency in other to stay ahead in the market when it comes to Vehicle_Efficiency and drive more Patronage*

*2.) They also want to know which demographics should they target for increase revenue and retention*


***METHOLOGY***

 *PYTHON: I used Python Pandas to cleaned, Organise and Matplotlib to visualised the data*
 


***SKILLS***
*Python: Pandas,Matplotlib, Seaborn, Visualising the dataset*
*I used the above liberies in Python to:*

- *Load and Inspect the dataset*
- *Handle missing values in the dataset*
- *And as well as removing duplicates and nulls*



  ***THE ANALYSIS CODES***
  
  ```PYTHON
  import pandas as pd
  pd.read_excel(r"C:\Users\USER-PC\Desktop\ALL ORIGINAL DATA FILES\automobile_data .xlsx")
  genius = pd.read_excel(r"C:\Users\USER-PC\Desktop\ALL ORIGINAL DATA FILES\automobile_data .xlsx")

  genius.groupby(["fuel_system"])[["city_mpg","highway_mpg"]].agg(["mean","count"]).plot(kind = "bar", title = "Fuel_System By MPG")

  genius[genius["fuel_type"]=="diesel"]

  

***KEY FINDINGS***

*Visualising the data and creating charts to track Vehicle_efficiency and performance to give Manufacturersa clear picture
into how they can improve Fuel_Types efficiency and maximise market opportunities. The following were my findings from this Automobile dataset*

*1.) This analysis shows that each Vehicle makes and their cost, fuel_type and fuel_system varies.*
*2.) The analysis also show us the make with the highest number of Vehicle base on cost and horsepower etc.*

<img width="542" height="472" alt="image" src="https://github.com/user-attachments/assets/43da01c0-f9e2-4571-9926-971926dcc4e2" />



   
***BUSINESS RECOMMENDATIONS***

*1.) ***ENGINE OPTIMISATION:*** The Brand is advice to design and optimise engines to run efficiency on specific fuel types such as gasoline,diesel, or other alternative fuel like ethanol.*

*2.) ***FUEL INJECTION SYSTEM:*** Implementing advanced fuel injection systems, such as direct fuel injection to improve efficiency and reduce emission is also a better way to go*

*3.) ***HYBRID AND ELECTRIC VEHICLE:*** Develop hybrid & electric vehicles that reduces dependence on fossil fuel will also improve efficiency etc etc*


***NEXT STEP***

*The next step I recommend for the Business is to focus Hybrid system Vehicle more as it improve more efficiency and drive more sells*
