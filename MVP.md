# Minimum Viable Product

### Background
Stanley at Fred & Mabel Yarns wants to determine a good price for his sweater patterns. I am using the website Ravelry.com to help him.

### MVP
The original webscraping included 2448 sweater patterns, but after dropping all the free patterns, patterns that are not priced in US dollars, and patterns not in English, I am left with 837 patterns. There are 16 features to predict price. One feature (yarn_weight) needs to be converted to a dummy variable, resulting in 27 features. I split the data into training (60%), validation (20%), and test (20%). With the 28 features, R^2 on the training data is 0.25; on the validation data it drops to 0.17, suggesting overfitting. 

However, even after correcting for overfitting, I do not expect to get better predictive results than the current R^2, as demonstrated by the plots below. These show each of the continous variables plotted against price for all 837 items; there is not a strong linear relationship in any of them. 

<img src="https://raw.githubusercontent.com/cda913/Regression_Metis/main/continuousVsPrice.png" width="600" height="300" />

### To Do
- Find which variables are really useful; the sheer number of variables is probably a part of the overfitting. 
- Cross-validation instead of mere fitting. 
- Look at a combination of variables that may be more predictive
