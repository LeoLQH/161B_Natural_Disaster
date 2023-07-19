# EDA & Data Visualizations

As we are interested in changes over the years, most of the variables would be graphed with years. Total damage discussed in this document would be total damage, adjusted by inlfation for 2018 dollars. 

Relevant variables include: disaster type, number of associated disastes, number of days, total deaths (binary), number injured (binary), number homeless (binary), disaster magnitude (binary) (reason on why they are used as binary is documented in the jupyter notebook - Data cleaning and processing)

We first graphed the number of natural disasters by year and its total damages over the years: 

<img width="971" alt="Number of Disasters by year" src="https://github.com/LeoLQH/161B_Natural_Disaster/assets/125975253/778762f7-0148-44fd-8fb8-503d6dd1845d">
`_Number of disasters by year_`

We can see there is a trend of increases in the number of natural disasters. We would verify this using statistical test - Pearsons's correlation coefficient - later.

<img width="971" alt="Summary of disaster cost by year" src="https://github.com/LeoLQH/161B_Natural_Disaster/assets/125975253/ad0e5c6d-59db-4e07-ae6e-063ca8edcf8e">

Sum of total damage, grouped by year

This is sum of the original total damage. Based from the graph, we would not expected much of a linear relationship. However, as stated during the cleaning process, money data are usually has big discrepancy between the lower values and bigger ones, so a natural log transformation was used to transform the data to be better analyzed.

We then graphed a scatter plot between the log of the data and year. As sum the log of the data would mean differently then log of the sum of the data (sum of log != log of sum), we do not graph on the sum of the log. 

<img width="500" alt="Log of damage adj by scatter plot" src="https://github.com/LeoLQH/161B_Natural_Disaster/assets/125975253/c19133c9-78ab-4bc8-a0c4-4ee7f4f1c53f">

From the graph, there seems to be a relationship and it can be a linear one, albeit not strong. We would also test this later. 

We then graphed other relevant variables with year:

Disaster type and year grouped by year (count):

<img width="500" alt="Number of disasters by type" src="https://github.com/LeoLQH/161B_Natural_Disaster/assets/125975253/c7b154ce-f26d-4e21-a36c-f4b1fb0bd5b2">

Disaster type and year on the log of total damages:

<img width="500" alt="Log of damage adj by type scatter plot" src="https://github.com/LeoLQH/161B_Natural_Disaster/assets/125975253/b8e8546f-49a4-482c-83e9-6a2313c20944">

This shows that there might not be a strong linear relationship between year and disaster type on log of total damage. 





