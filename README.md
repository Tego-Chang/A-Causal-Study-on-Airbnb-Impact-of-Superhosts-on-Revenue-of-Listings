# A-Causal-Study-on-Airbnb-Impact-of-Superhosts-on-Revenue-of-Listings
 
Team: FR-Schwartz, Jaya Khan, Satvik Kishore, and Tego Chang

In this study, we like to investigate if there's a causal effect between whether the host of a listing is superhost or not and the annual revenue of the listing. 

## Outline 

### Data Preprocessing
In the first phase, we preprocessed the dataset from Airbnb, including:
1. Exclude the irrelevant or uninterested features and implement feature engineering.
2. Handling missing data.
3. Define the response variable and calculate based on existing features.
4. Reduce the chance of having multicollinearity issues (as we treat this study as a linear regression problem).

### Apply Dame for Matching
In the second phase, in order to ensure the form of our model assumption will not generate a biased result, we conduct matching using Dame. This phase includes preprocessing and postprocessing the dataset as input for Dame and output for the following model section correspondingly.

### Statistical Modeling
In the third phase, we built statistical models and investigate the coefficients of *host_is_superhost* and other exploratory variables and their relationships with our response, annual revenue of listings. Meanwhile, we also ensure the assumptions of linear regression are well met. In our final model, we consider *host_is_superhost* as a fixed effect and cluster its standard error so that besides our question of interest, the causal effect of superhost on annual revenue, we could also have a more precise estimate of the impact of other exploratory variables on our response.

### Visualization of Results
In the last phase, we visualized the outcome of our model, and we found the host status, being a superhost or not, of a listing indeed plays an obvious effect on the annual revenue of the listing. Further, other features' impacts on the response are also demonstrated. 
