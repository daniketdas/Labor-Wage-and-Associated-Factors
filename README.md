# Labour-Wage-and-Associated-Factors
## Objective:
In this project, I delved into the intricate relationship between labour wages and various influencing factors. The objective was to comprehensively analyse the determinants that impact wages across different industries and demographics. By examining this multifaceted landscape, we aimed to gain valuable insights into the dynamics of labour compensation and its implications for workforce management, economic policies, and social equity. This is a study where we will see the association between labour wage and other factors (usual working hour, total experience and tenure) based on the data of 2246 labours taken from 1988 survey. 
## Data Source:
Now to estimate the parameters we have used the data collected from 2246 labours on the survey of 1988 regarding the mentioned variable. 

## Prior Studies on This Topic:
![image](https://github.com/daniketdas/Labor-Wage-and-Associated-Factors/assets/162815966/d1ada208-5e4c-4786-aa81-83ce63e8e1e6)
## Research Question:
**How factors like total working hour, experience and tenure influence labour wage?**

Here we are trying to find out how wage is dependent on time at work and other various variables like total experience and tenure.
## Econometric Model:
Here we are taking wage (monthly wage) as the dependent variable and other variables such as hours (usual hours worked), ttl_exp(total work experience), tenure (job tenure in years)as independent variable.  
So, the econometric model will be,  
![image](https://github.com/daniketdas/Labor-Wage-and-Associated-Factors/assets/162815966/83aeed30-d19b-4c71-8d2f-f0fcc00feb4c)

(Here  is the intercept and  are coefficients of the variables and  is the error term.)
## Estimation and Interpritation of The Result:
![image](https://github.com/daniketdas/Labor-Wage-and-Associated-Factors/assets/162815966/1b746d1f-2013-4d9e-b742-39a852677e3c)

1)Coefficient of hours is positive, it means if there is an increase in usual working hours of female, the wage of them will also increase.
2)Coefficient of total work experience (ttl_exp) is positive, that means if total work experience increases, their wage will also increase. 
3)Coefficient of job tenure is also positive, that means if tenure increases wage will also increase.
## Statistical Significance of Variables:
![image](https://github.com/daniketdas/Labor-Wage-and-Associated-Factors/assets/162815966/f9213703-f6f1-4bd9-9729-213aa4244069)

So, we can see that out of these 3 independent variables 2 are statistically significant (since their P>|t| values are less than 0.05 or they do not have 0 in their confidence interval.)
Thus, we can see that only ‘hours and ttl_exp’, these two variables are statistically significant.

![image](https://github.com/daniketdas/Labor-Wage-and-Associated-Factors/assets/162815966/1ca9dcb4-8c9e-480a-8504-e644326ef0a2)

In order to check that we need see P>F value, here prob>F value of this model is 0.000, that means all the slope parameters are jointly not equal to 0, at least one slope parameter is non-zero in this model. Yes, there is an evidence of regression relationship as 2 independent variables are significant in this model.
By the value of R-squared we can say that this model is capable of explaining approximately 7.99% of the variation in wage (dependent variable).

## Heteroscedaticity Check:
Now to check if there is heteroscedasticity in the model, we have taken use of Breusch-Pagan/Cook-Weisberg test of heteroscedasticity. So, here from our test we can see that null hypothesis of constant variance is rejected as the Prob > chi2 value is less than 0.05 so we can conclude that the variance of the error term is not constant so there is heteroscedasticity in the model and that is why the estimates obtained above are biased and we cannot rely on those estimates. So, we have to make sure that constant variance is maintained and to maintain this we have to use another estimator which is WLS (weighted least square). Here we assign a weight variable and put weights on the variables then we again run OLS on those weighted variables and in this way estimated values will not be biased anymore as the variance becomes constant.

## Conclusion:
In wrapping up our project, we've learned a lot about what affects how much people get paid. We found that working more hours generally means higher pay, and as people gain more experience and stay in their jobs longer, their pay tends to go up too.
However, we need to remember that our findings have some limitations. The data we used might not be perfect, and there could be other factors we didn't consider that also play a role in determining wages.
Moving forward, it's important to keep studying this topic to get a clearer picture. By improving our methods and looking at more factors, we can better understand how wages are set and work towards making sure everyone is paid fairly.
Overall, our project adds to the conversation about how to create fairer and more inclusive job markets, where everyone has the opportunity to earn a decent wage.

