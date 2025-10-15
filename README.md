# Assignment2
## by Evelyn Bushell

## Description of dataset
I am using a dataset of King County's housing sales from 2014-2015. The target variable will be pricing as that is the most likely to be dependent on other features

## Data cleaning and feature engineering
I noticed that while there is no explicitly missing data, there are some rows with Price listed as 0. After checking to see how much of my data this encompasses, I have dropped these rows as I believe they represent unsold houses. I also noticed that Price was very right skewed so I performed a logarithmic transformation of it, replacing the original column.[br]
As my feature engineering, I decided that square footage of lot would have the best indicators for price. This was also right skewed, so I made a separate column of this data when it was logarithmically transformed as well.

## Final evaluations
My metrics were a very mixed bag. My R2 score was very low (0.01) however my MSE score was also very low (0.28). After viewing the scatterplot, it looks like while the model did its best to fit its regression line, using just one feature for the model results in very noisy data.