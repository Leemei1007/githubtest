# Project 2 - Ames Housing Data and Kaggle Challenge


#### Problem statement
- The client is a mid-size real estate agency. 
- Since its establishment more than a decade ago, it has closed numerous real estate deals and kept detailed records of such real estate sold.
- As part of its digitalisation initiatives, the client is keen to monetise its dataset. It wishes to outsource the development of an in-house model to predict the sale price of real estate in that area.
- Such model is meant to assist its real estate agents in their selling and marketing activities. If the real estate agent can help give potential housebuyers some insight of selling prices or what features to look out for to justify sale prices, such capability can boost the competitiveness of the agency in the long run.  

#### Objectives
- To develop a linear regression model to predict sale prices of residential real estate
- The model to be develop will have a target R-squared score of above 70% (Note - R-squared is the percentage of the dependent variable (in this case, features / characteristics of the real estate) variation that a linear model explains)
- The model is not meant to be foolproof. The model is to help guide real estate agents in their selling and marketing activities. The users of the model are expected to exercise some judgement when using the model. There are scenarios where the model may not be relied upon in its entirety, for eg. selling the property in an auction process. In times like this, the Sale Price will be a 'firesale', not based on market price.    

#### Overall workflow
- The process of developing the model entail the following:
1. Importing the dataset for the purposes of training the model
2. Prepping the data, i.e. data cleaning, inpute the missing values, feature engineering, which include dealing with outliers and categorical data, add additional data.
3. Some preliminary EDA conducted to gauge relationship
4. Data modelling - 3 models were compared, namely, Linear Regression Model, Ridge Regression and Lasso Regression Model. Turns out, the worst performing model was the Linear Regression Model. This could be due to the multicollinearity of the features. To address the issue of multicollinearity, Lasso Regression Model was adopted.

#### Conclusion

#### Model choice

- The Lasso Regression model is the model with the best score among Linear Regression and Ridge Regression


#### Important features from final Lasso Regression model 

We can conclude that size and quality of the real estate contribute positively to Sale Price while age of the building is the main negative feature that contribute negatively to Sale Price

|Top 5 Positive Feature       | Coefficient  | 
|---------------|--------------|
| Gr Liv Area |  26645.740994  | 
| Overall Qual |  12013.833702    | 
| BsmtFin SF 1 | 9686.420937    | 
| Total Bsmt SF | 7163.438230| 
| Neighborhood_NridgHt | 6295.01764   | 


| Top 5 Negative Feature       | Coefficient  | 
|---------------|--------------|
| Building age |  -8496.417470  | 
| MS SubClass_120 |  -4064.612134    | 
| MS SubClass_160 | -3894.699231    | 
| Mas Vnr Type_BrkFace | -3685.764617| 
| Bedroom AbvGr | -2689.418166  | 	

#### Recommendation

- The Client (i.e. the real estate agency) may adopt the Lasso Regression Model
- Users of the model (i.e. the real estate agents) may use the model to gauge Sale Price. Once Sale Price is established, the user may use this benchmark price as base price for negotiation or look out for a good deal in the market.
- Real Estate Agents may use this model to advise homeowners on how to improve selling prices of the house by referring to the coefficients. For eg, remodel the house to improve overall quality or extend the size of living area or basement to boost selling price.