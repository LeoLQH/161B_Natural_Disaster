# Results and Models

Based on our model, we found sufficient evidence to suggest there is a linear relationship between year and log of total damages, with a Pearson's correlation coefficient R of ~ .196 . The bivariate fit of year and log of total damages has found a statistically significant regarding year and log of total damages. However, as R is low, it would results in an even lower R^2. This suggests there might be other variables at play in the linear model. Thus, we adopt a multiple linear regression instead. 

We first tried to fit a multiple regression model without any interactions term. This gives us a model with all parameters being statistically significant. The goodness of fit test also returned a value indicating there the model describes the data relatively well. 

<img width="531" alt="Full model - Simple Parameter Ests" src="https://github.com/LeoLQH/161B_Natural_Disaster/assets/125975253/3534f6ff-2b61-4f06-98ff-e3ac0e8eb8ff"> 

However, the R^2 from this model shows that the model explains not much of the variability of the actual data. Furthermore, many of the predictor variables are statistically significant in their correlation, thus we explore adding multiple interactions terms.  

As we use the standard least squares method, we tested the potential correlations between the predictors to account for potential multicolinearity. Additionally, many of the variables are nominal with 2 to 3 categories. Again to mitigate for multicolinearity, we used one of the categories from each variables as the reference. The fullest model (model with all possible interaction terms) is captured here: 

<img width="573" alt="Full Model Parameter Ests" src="https://github.com/LeoLQH/161B_Natural_Disaster/assets/125975253/7e2280cc-b077-422d-82f7-2773f6a7a2de">

Despite an increase in R^2, it is too modest considering the complexity of the new model. We then explored new models using only interaction terms with our main predictor variable, year. The results are not much different. They are capture here: 

<img width="573" alt="Full Model - Simple with year interaction terms" src="https://github.com/LeoLQH/161B_Natural_Disaster/assets/125975253/cbd711bc-61e2-4c17-b804-7e8521dcae1e"> 

The model became more complex while there is not really any practical change. 

Additionally, we also controlled for different disaster types, deriving models from them to see how good they are. Of them, year is found to be significant only to Storms. However, R^2 is consistently lower in all of them than using disaster type of as a predictor. 

Hence, overall, we chose to stick to the simplest models to ensure interpretability and model efficiency. Yet, note that the R^2 is still really low, meaning year and other variables do not account for a large portion of the increase in the damage of natural disasters.

This also mean that a prediction model, as set out in the research question, is not reliable, from the current set of variables we used. 
