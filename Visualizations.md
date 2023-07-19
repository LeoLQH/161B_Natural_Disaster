# EDA & Data Visualizations

As we are interested in changes over the years, most of the variables would be graphed with years. The total damage variable discussed in this document would be total damage, adjusted by inflation for 2018 dollars. 

Relevant variables include: disaster type, number of associated disasters, number of days, total deaths (binary), number injured (binary), number homeless (binary), disaster magnitude (binary) (reason on why they are used as binary is documented in the jupyter notebook - Data cleaning and processing)

We first graphed the number of natural disasters by year and their total damages over the years: 

<img width="971" alt="Number of Disasters by year" src="https://github.com/LeoLQH/161B_Natural_Disaster/assets/125975253/778762f7-0148-44fd-8fb8-503d6dd1845d">
Number of disasters by year

We can see that there is an increasing trend in the number of natural disasters. We would verify this using statistical test - Pearsons's correlation coefficient - later.

<img width="971" alt="Summary of disaster cost by year" src="https://github.com/LeoLQH/161B_Natural_Disaster/assets/125975253/ad0e5c6d-59db-4e07-ae6e-063ca8edcf8e">

Sum of total damage, grouped by year

This is the sum of the original total damage. Based on the graph, we would not expect much of a linear relationship. However, as stated during the cleaning process, money data usually has a big discrepancy between the lower values and the bigger ones, so a natural log transformation was used to transform the data to be better analyzed.

We then plotted a scatter plot between the log of the data and year. As sum the log of the data would mean differently then log of the sum of the data (sum of log != log of sum), we do not graph on the sum of the log. 

<img width="500" alt="Log of damage adj by scatter plot" src="https://github.com/LeoLQH/161B_Natural_Disaster/assets/125975253/c19133c9-78ab-4bc8-a0c4-4ee7f4f1c53f">

From the graph, there seems to be a relationship, and it can be a linear one, albeit not strong. We would also test this later. 


We then graphed other relevant variables with year

Disaster type and year grouped by year (count):

<img width="541" alt="Number of disasters by type" src="https://github.com/LeoLQH/161B_Natural_Disaster/assets/125975253/23ca4c23-b49e-4e27-81eb-7156459d4f6e"> ()
 
Number of days and year: There seems to be a strong linear relationship between years and the number of days the disaster went on for ()

<img width="700" alt="Number of days and year" src="https://github.com/LeoLQH/161B_Natural_Disaster/assets/125975253/7a481274-1ffc-4dcd-95e7-a85dccb8fabd"> ()

Number of associated disasters and year: It is obvioous that there are more and more associated disasters as years go by. ()

<img width="700" alt="Number of associated disasters and year" src="https://github.com/LeoLQH/161B_Natural_Disaster/assets/125975253/9bfbe844-2a4d-428a-af34-86e3924b6e80"> ()


Total death (binary) and year: Many recent cases reported having aat least one death. This would be analyze through a logistic regression model and a decision on whether it will enter the model will be made accordingly. ()

<img width="700" alt="Total death binary and year" src="https://github.com/LeoLQH/161B_Natural_Disaster/assets/125975253/e74b9040-cecd-4798-9488-d41ae4be5ab9"> ()


Most of the potential correlations shown here were tested using various statistical tools such as the F-test, t-test, Pearson correlation coefficient, and logistic regression. The explicit result of the test will not be shown.


