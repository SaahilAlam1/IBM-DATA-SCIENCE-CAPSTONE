# IBM-DATA-SCIENCE-CAPSTONE
In this capstone, we will predict if the Falcon 9 first stage will land successfully. SpaceX advertises Falcon 9 rocket launches on its website, with a cost of 62 million dollars; other providers cost upward of 165 million dollars each, much of the savings is because SpaceX can reuse the first stage. Therefore if we can determine if the first stage will land, we can determine the cost of a launch. This information can be used if an alternate company wants to bid against SpaceX for a rocket launch. 

Explore:
  How payload mass, launch site, number of flights, and orbits affect first-stage landing success
  Does a launch site’s location and proximity affect the success rate?
  Best predictive model for successful landing


Executive Summary:
  Methodologies:
  Data collected through web scraping and using SpaceX REST API 
    Performed data wrangling to created successful/fail outcome variable
    Carried out exploratory data analysis using SQL and data visualization
    Built a dashboard visualizing launch sites with the most success and successful payload ranges
    Built classification models to predict landing outcomes using logistic regression, support vector machine, K-nearest neighbor and decision tree
  Results:
    Launch success has improved throughout the years
    KSC LC-39A has the highest success rate among landing sites
    Payload Mass contributed most to the chances of a launch being successful given the type of orbit type and booster version
    Orbits ES-L1, GEO, HEO, and SSO have a 100% success rate
    Most launch sites are close to the coast
    All models performed similarly on the test set where the decision tree model slightly outperformed


Conclusion:
  Model Performance: 
    The models performed similarly on the test set with decision tree model slightly outperforming
    All launch sites are located near the coast
    The launch success increase over time
    The greater the payload mass, the greater the chances of the launch being successful for all launch sites
    Orbit type ﻿ES-L1, GEO, HEO, and SSO have a 100% success rate
    Booster version ‘FT’ and ‘B4’ have the highest success rate for payload mass range between 2000 and 5500 kg
    Launch site KSC LC-39A has the most successful launches, while CCAFS LC-40 has the lowest success rate
  Additional Things to Consider:
    Dataset: A larger dataset will help build on the predictive analytics results to help understand if the findings can be generalizable to a larger data set
    Feature Analysis / PCA: Additional feature analysis or principal component analysis should be conducted to see if it can help improve accuracy
    XGBoost: Is a powerful model which was not utilized in this study. It would be interesting to see if it outperforms the other classification models
