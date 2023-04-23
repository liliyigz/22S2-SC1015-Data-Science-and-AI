# Hypertension Classifier using Machine Learning and Optimisation Techniques
![hypertension](https://user-images.githubusercontent.com/88404898/233834788-46a0b9cb-908b-4b1c-b60d-36fa5b22f859.png)
## About
This is the Mini-Project done for SC1015 Introduction to Data Science and Artificial Intelligence. In this project, we aim to identify individuals with high risk of hypertension who are undiagnosed, using Data Science and Machine Learning algorithms. 

The dataset we chose is taken from 2021 Behavioural Risk Factor Surveillance System Survey Data and Documentation conducted by US Centers for Disease Control and Prevention (CDC).

The documents and source codes are presented in the following order:
1. [Data Extraction & Cleaning](https://github.com/liliyigz/22S2-SC1015-Data-Science-and-AI/blob/bcf2ffa4efe45d0f024e1c2dc7efe0bb94fc290d/1.%20%5BData%20Extraction%20&%20Cleaning%5D.ipynb)
2. [Exploratory Data Analysis](https://github.com/liliyigz/22S2-SC1015-Data-Science-and-AI/blob/bcf2ffa4efe45d0f024e1c2dc7efe0bb94fc290d/2.%20%5BExploratory%20Data%20Analysis%20and%20Visualization%5D.ipynb)
3. [Model 1: Decision Tree](https://github.com/liliyigz/22S2-SC1015-Data-Science-and-AI/blob/bcf2ffa4efe45d0f024e1c2dc7efe0bb94fc290d/3.%20%5BModel%201:%20Decision%20Tree%5D.ipynb)
4. [Model 2: Random Forest](https://github.com/liliyigz/22S2-SC1015-Data-Science-and-AI/blob/bcf2ffa4efe45d0f024e1c2dc7efe0bb94fc290d/4.%20%5BModel%202:%20Random%20Forest%5D.ipynb)
5. [Model 3: Logistic Regression](https://github.com/liliyigz/22S2-SC1015-Data-Science-and-AI/blob/bcf2ffa4efe45d0f024e1c2dc7efe0bb94fc290d/5.%20%5BModel%203:%20Logistic%20Regression%5D.ipynb)
6. [Dataset & Codebook]

## Contributors
### Team:
Practical Motivation & Problem Formulation
### Li Liyi:
Decision Tree with Optimisation
### Wu Rixin:
Data Cleaning, Exploratory Data Analysis & Analytic Visualisation
### Yong Shao En Ernest:
Random Forest with Optimisation & Logistic Regression with Optimisaion

## Problem Definition
In Singapore, hypertension is the most common medical condition, with 35.5% of adults being diagnosed in 2020. Hypertension is also the leading risk factor for cardiovascular disease and death globally, and untreated hypertension can lead to heart disease which can be fatal. 

This leads to our problem statement: 
<b>What are the variables correlated with hypertension and how can we identify undiagnosed individuals suffering from hypertension?</b>
- How can we identify undiagnosed individuals suffering from hypertension?
- Which models are most suitable for machine learning?

## Data Cleaning and Preparation
<p>Data cleaning and preparation are crucial steps in the data analysis process. These steps involve transforming raw data into a format that is suitable for analysis, and ensuring that the data is accurate, complete, and consistent. </p>

Key steps involved in our data cleaning and preparation process include:
1. Extract columns that are relevant to our problem, i.e., hypertension analysis
2. Tackle missing values
3. Tackle irrelevant data entries
4. Create new variables by combining or transforming existing numeric variables
5. Decode categorical variables based on data description
6. Compute true values for numeric variables
7. Identify and remove outliers for numeric variables
8. Export cleaned dataset to csv

## Exploratory Data Analysis and Visualization
After data cleaning, Exploratory Data Analysis (EDA) and Visualisation are conducted to better understand the variables and obtain initial data-driven insights on their relationships with hypertension.

Key steps involved in our EDA and Visualisation include:
1. Uni-variate analysis and visualisation for both numeric and categorical variable
2. Bi-variate analysis and visualisation to identify promising predictor numeric variables via boxplots
3. Bi-variate analysis and visualisation to identify promising predictor categorical variables via catplots

## Machine Learning Models
The models were chosen by considering the large data set and the high number of categorical variables. The following models were used:

### 1. Decision Tree
- Constructing a model of decisions and their possible consequences
- Optimising depth level using AUC value of ROC Curve

### 2. Random Forest
- Using multiple decision trees to diversify train data set 
- Optimising depth level using AUC value of ROC Curve

### 3. Logistic Regression
- Predicting output of a categorical variable based on multiple independent variables
- Optimisation through hyperparameters
- Identifying best hyperparameters through GridSearch

## Conclusion
- A correlation between arthritis and hypertension was found although the link cannot be explained by scientific knowledge.
- A higher proportion of black people suffer from hypertension compared to all other racial demographics. This suggests that hypertension can be caused by genetic factors.
- People with and without hypertension have the same average intake of fruits and vegetables. This suggests that there are other more significant factors that contribute to hypertension.
- Cholesterol, BMI and age are the three most significant contributors to hypertension based on our 3 models. 

## References

### Data Source
https://www.cdc.gov/brfss/annual_data/annual_2021.html</br>
To download the raw data file, please access: https://www.dropbox.com/s/veea7xd97rc7kdv/raw.csv?dl=0

### Machine Learning
https://scikit-learn.org/stable/modules/tree.html
https://developers.google.com/machine-learning/crash-course/classification/roc-and-auc
https://www.section.io/engineering-education/introduction-to-random-forest-in-machine-learning/#:~:text=What%20is%20a%20random%20forest,consists%20of%20many%20decision%20trees
https://scikit-learn.org/stable/modules/generated/sklearn.linear_model.LogisticRegressionCV.html
https://www.kaggle.com/code/funxexcel/p2-logistic-regression-hyperparameter-tuning/notebook

### Secondary Research
https://www.moh.gov.sg/docs/librariesprovider5/default-document-library/nphs-2020-survey-report.pdf
https://my.clevelandclinic.org/health/articles/11918-cholesterol-high-cholesterol-diseases#:~:text=Cholesterol%20plaque%20and%20calcium%20cause,biggest%20causes%20of%20heart%20disease
https://www.cdc.gov/bloodpressure/about.htm#:~:text=The%20higher%20your%20blood%20pressure,%2C%20heart%20attack%2C%20and%20stroke
https://www.cdc.gov/bloodpressure/about.htm#:~:text=The%20higher%20your%20blood%20pressure,%2C%20heart%20attack%2C%20and%20stroke
https://www.medicalnewstoday.com/articles/hypertension-and-asthma#:~:text=People%20with%20asthma%20are%20more,developing%20hypertension%20and%20heart%20disease
https://www.amjmed.com/article/S0002-9343(09)00208-3/fulltext#:~:text=Arthritis%20pain%20often%20occurs%20concurrently,to%20treat%20pain%20and%20inflammation
https://www.ncbi.nlm.nih.gov/pmc/articles/PMC4108512/
https://www.ncbi.nlm.nih.gov/pmc/articles/PMC4703088/
