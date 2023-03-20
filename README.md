# Data-Analysis-on-Filipino-Family-Income-and-Expenditure
The dataset was sourced through kaggle from the Philippine Statistics Authority's (PSA) Family Income and Expenditure Survey (FIES) nationwide. The survey, which is undertaken every three (3) years, is aimed at providing data on family income and expenditure, including, among others, levels of consumption by item of expenditure, sources of income in cash, and related information affecting income and expenditure levels and patterns in the Philippines.

The Dataset contains more than 40k observations and 60 variables which is primarily comprised of the household income and expenditures of that specific household. For this analysis, I will be using Python's pandas, numpy, and hvplot libraries.

The following questions/objectives are being sought:
1. What is the Average Yearly Food Expenditure and Average Income per region? Which region has the highest and lowest?
2. What is the ratio of Food Expenditure to income per region? Which region has the highest and lowest?
3. Scatter plot of Household Income and Total Food Expenditure in the Philippines
4. Scatter plot of Househoold Income and Ratio of Food Expenditure to Income
5. What are the main sources of income in the country? Per region?
6. What are the proportions of the sources of income per region?
7. How much does each region spend on other expenses?
8. Head Sex per Region and Overall
9. Household Head Age distribution
10. What is the Mean Age?
11. Regions sorted by Total Income from Entrepreneurial Activities
12. What is the Correlation of Income and Expenditures?

Results: 
1. It is evident that the National Capital Region (NCR) has the highest Average Household Income (420K) and the Highest Average Food Expenditure (127K). Moreover, the Autonomous Region of Muslim Mindanao (ARMM) has the lowest Average Household Income (134K) while Northern Mindanao the lowest Average Food Expenditure (64K). 
![regions yearly income expenditure](https://github.com/johanncatalla/Data-Analysis-on-Filipino-Family-Income-and-Expenditure/blob/main/images/1.png)
2. In terms of Ratio of Food Expenditure to Income, SOCCSKSARGEN has the highest ratio with 0.55, meaning 55% of their income goes to food. On the other hand, the region with the lowest ratio is NCR with 0.37 or 37%. Despite having the highest income and highest food expenditure, NCR has the lowest ratio of food to income, which implies that their other expenses are marginally more prioritized compared to other regions. It can be observed that lower-income regions are more likely to allot a higher percentage of their income to food expenditures. Similarly, higher-income regions are more likely to have a lower percentage of their income allotted for food expenditures. 
![food ratio to income](https://github.com/johanncatalla/Data-Analysis-on-Filipino-Family-Income-and-Expenditure/blob/main/images/2.png)
3. We can observe the first scatter plot of Total Household Income and Total Food Expenditure to find the correlation. It can be seen that the two variables has a positive linear correlation (indicated by the upper-inclined pattern) which means that as income increases, Food Expenditure also increases.

![scatter income expenditure](https://github.com/johanncatalla/Data-Analysis-on-Filipino-Family-Income-and-Expenditure/blob/main/images/3.png)

4. In the second scatter plot, I plotted the Total Household Income as x and Ratio of Food Expenditure to Income as y. It can be observed that it has a negative linear correlation (indicated by the lower-inclined pattern) which means that as Income Increases, the Ratio of Food Expenditutre to Income decreases. This tells us higher-income houseolds spend a lower percentage of their income for food. 
![scatter income ratio](https://github.com/johanncatalla/Data-Analysis-on-Filipino-Family-Income-and-Expenditure/blob/main/images/4.png)
5. In the first bar graph, it can be observed that Wage/Salaries is the main source of income Filipino Households while Entrepreneurial Activities being the lowest. It is evident in the second bar graph that Wage/Salaries are the main sources of income per region, except in ARMM. The next bar graph will show the proportions of each source of income.
![PH main source of income](https://github.com/johanncatalla/Data-Analysis-on-Filipino-Family-Income-and-Expenditure/blob/main/images/5.1.png)
![Region main source of income](https://github.com/johanncatalla/Data-Analysis-on-Filipino-Family-Income-and-Expenditure/blob/main/images/5.2.png)
6. The Following Conclusions can be made: 
    1. ARMM is the only region with Entrepreneurial Activities being the Main Source of Income (0.78 or 78%). 
    2. NCR has the highest ratio of Wage/Salaries as main source of income (0.68 or 68%)
    3. NCR has the lowest ratio on Entrepreneurial Activities (0.125 or 12.5%)
    4. All regions except ARMM has Wage/Salaries as their Main Source of Income.
![ratio source of income per region](https://github.com/johanncatalla/Data-Analysis-on-Filipino-Family-Income-and-Expenditure/blob/main/images/6.png)
7. The following conclusions can be made: 
    1. NCR has the highest housing and water, house rental, transportation, clothing and footwear, communication, education, restaurant and hotels, and miscellaneous goods and services expenditures.
    2. NCR has the lowest crop farming/gardening expenses. 
    3. ARMM holds the highest crop farming/gardening expenses and lowest expenditure for the rest of the categories. 
    4. Cagayan Valley and Cordillera Administrative Region (CAR) has the second and third highest expenditure on crop farming/gardening respectively.
    5. CALABARZON holds the highest expenditure for special occasions and medical care. 
    6. NCR has the highest overall expenditure for other expenses.
![other expenses](https://github.com/johanncatalla/Data-Analysis-on-Filipino-Family-Income-and-Expenditure/blob/main/images/7.png)
8. It can be observed that across the regions and the country, the majority of household head sex is male. 
![head sex per region](https://github.com/johanncatalla/Data-Analysis-on-Filipino-Family-Income-and-Expenditure/blob/main/images/8.1.png)
![head sex PH](https://github.com/johanncatalla/Data-Analysis-on-Filipino-Family-Income-and-Expenditure/blob/main/images/8.2.png)
9. It can be observed that the bar graph ranging from ages 9-99 forms a bell curve, with a mean age of 51.
![head age PH](https://github.com/johanncatalla/Data-Analysis-on-Filipino-Family-Income-and-Expenditure/blob/main/images/9.png)
10. The mean age is 51.381450991719625
11. It can be concluded that ARMM has the highest Total Income from Entrepreneurial Activities while Bicol Region has the lowest. 
![entrepreneurial activities region](https://github.com/johanncatalla/Data-Analysis-on-Filipino-Family-Income-and-Expenditure/blob/main/images/11.png)
12. The heatmap plots the correlation between the variables of Expenses together with the Total Household Income and Food Percentage to Income. It can be observed that Ratio of Food Expenditure to Income and Total Household Income has a moderately strong negative correlation (0.44), which confirmed our findings earlier. Furthermore, Total Food Expenditure and Total Household Income has a strong positive correlation (0.66) which also confirmed our findings. The following conclusions can be made:
    1. Total Household Income has a significant effect to Total Food Expenditure. Higher-income household are more likely to spend more on food.
    2. Total Household Income has a significant effect to Ratio of Food Expenditure to Income. Higher-income households are more likely to have a lower percentage of their income allotted for food expenditures. Similarly, lower-income households are more likely to allot a higher percentage of their income for food expenditures.
    3. Total Household Income has a significant effect to Other Expenses. Higher-income households are more likely to spend more on expenses other than food.  
![heatmap correlation income expenditure](https://github.com/johanncatalla/Data-Analysis-on-Filipino-Family-Income-and-Expenditure/blob/main/images/12.png)
