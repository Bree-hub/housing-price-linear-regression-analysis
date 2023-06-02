# Housing Price Linear Regression Analysis

**Authors:**
 1. Julius Charles
 2. Brenda Kinoti
 3. cleophas Opati
 4. Winnie Onduru
 5. John Karanja
 6. Joy Wangari
 7. Jonathan Okwaro

**Client:** Yuniq Realtors

## Overview
In this project, linear regression analysis is employed to examine the influence of specific variables on housing prices and determine the extent of their impact. By analyzing data from King County House Sales, it is revealed that the condition of the house, its grade, and the number of bathrooms are significant factors that contribute to higher prices. This information can be valuable for homeowners looking to sell their properties as it enables them to make informed decisions regarding potential renovations or improvements.

## Business Problem
The client aims to create a platform that provides accurate house price estimates for buyers and sellers in King County.They need a platform where buyers and sellers will have access to reliable price estimates, enabling them to make informed decisions during property transactions.

## Data
This project uses 2014-2015 data from the King County House Sales dataset. It includes information on over 21,500 houses describing features such as year of renovation,space,number of bedrooms condition, etc.

## Method
The analysis deployed in this project uses multiple linear regression methods to develop a model of house price using a subset of predictor variables. Several variables were log transformed, and all non-binary variables were standardized. Model iterations were compared by r-squared score.

## Results
The final model has a r-squared score of 0.537, meaning that 54% of the variance in the dataset is described by the model.
Our final model also had a Root Mean Squared Error of 256128.9.
All model features had a p-value < 0.05 (our alpha/significance level), which tells us that all features have a statistically significant linear relationship with price.
The final model included 4 of the most significant predictor variables of house price. They are, Intercept, grade, sqft_living and bathrooms.
Our final model3 when compared to the baseline model, the R-squared increase from 50% to 54%

![RESULTS](./images/results.png)

## Conclusion
- **The model's ability to account for approximately 47% of the variability in house prices, as indicated by the R-squared value of 0.473, shows promise but acknowledges that there are other factors influencing house prices beyond the features included in the model.
- **The root mean squared error (RMSE) of approximately USD 256,129 highlights the model's average prediction deviation from the actual prices. While the model provides a useful tool for estimating house prices, it should be recognized that it is not perfect and can benefit from ongoing refinement and updates.
- **All of the selected features in our model exhibited statistically significant linear relationships with the price, as evidenced by their p-values being less than the chosen significance level. While we only barely met the assumption of homoscedasticity after standardizing the data, we satisfied the assumptions of independence, linearity, and normality.
- **Our analysis revealed that grade, square footage (sqft_living), and bathrooms were the most influential factors affecting house prices in King County. Homeowners seeking to maximize their selling price should focus on increasing the square footage and improving the quality of construction. Additionally, adding more bathrooms appears to have a positive association with price.
- **It is important to acknowledge the limitations of our model. Certain variables required log transformation to meet regression assumptions, which implies that any new data used with the model would necessitate similar preprocessing.
- **To enhance our understanding further, future analysis should explore the significant predictors of home prices in locations outside of King County and investigate homes with extreme price values. This would provide valuable insights into the factors driving housing prices in different regions and for properties with unique characteristics.
- **For a more comprehensive analysis of house sales, several additional steps can be taken. Firstly, considering alternative models, such as polynomial models, can capture non-linear relationships between predictors and the outcome, expanding beyond the limitations of linear models. Additionally, adjusting house sale prices for inflation would yield a more accurate understanding of trends and patterns in the housing market over time.
- **Lastly, collecting additional data in the coming years, particularly during periods of economic recession or interest rate hikes by the Federal Reserve, would allow for the analysis of how these factors influence house sales. This would provide valuable insights into the dynamics of the housing market and aid in making more informed predictions and decisions.

## Next Steps
- **Adjust house sale prices for inflation. By incorporating an inflation adjustment, the analysis can provide a more accurate understanding of the trends and patterns in house sales over time.
- **Collect additional data in the upcoming years, especially considering the potential economic recession and the possibility of interest rate hikes by the Federal Reserve. Analyzing how these factors impact house sales can provide valuable insights into the dynamics of the housing market.
- **Explore the relationship between individual predictors and the outcome variable, as they may not exhibit a linear relationship. This can be accomplished by considering alternative models such as polynomial models, which can better capture non-linear relationships between predictors and the outcome, instead of relying solely on linear models.

## For More Information

See the full analysis in the [Jupyter Notebook](./Student.ipynb) or review this [presentation](./presentation.pdf).


- **Our project provides valuable insights into the factors affecting house prices in King County and offers recommendations for homeowners and researchers interested in understanding the housing market dynamics.


