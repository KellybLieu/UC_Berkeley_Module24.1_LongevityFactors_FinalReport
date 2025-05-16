# UC_Berkeley_Module24.1: Longevity Factors
Author: Kelly Lieu <br/>

BACKGROUND <br/>
My goal is for this capstone is to learn and practice how to apply ML/AI techniques with data visualization tools. It was important to me to choose a dataset that was easy to obtain and a topic that I can learn from to apply at home or at work. The data comes from Kaggle called, "Longevity Factors." 
<br/><br/>
WE WILL EXPLORE <br/>
What longevity factors provide most gain in years of life?
What factors provide the most gain in years of life for females?
What are the top features based on the weighted impact of strength of science on years?
Which machine learning algorithm should I use with this specific dataset?
How can I improve my machine learning model?
<br/><br/>
SUMMARY OF EAD FINDINGS <br/>
The initial exploratory data analysis (EAD) involved loading and cleaning the dataset, identifying missing values, and removing irrelevant columns such as comments, notes, sources, and IDs. Visualization through histograms revealed that most longevity effects ranged from 2 to 6 years, with a few extreme negative outliers (e.g., -25 years). The majority of factors had weak scientific backing, and further statistical exploration (boxplots, pairplots) yielded limited insights due to the dataset’s low dimensionality and lack of strong correlations.
<br/>
Given the inconclusive initial results, a secondary analysis was conducted to assess the relationship between longevity factors and scientific strength, as well as to explore gender-based differences. A weighted impact score was calculated by multiplying the years gained/lost by the science strength rating (1–3), offering a clearer picture of each factor’s relative importance.
<br/>
The top science-backed positive longevity factors included:

<li>A combined healthy lifestyle (non-smoking, regular exercise, healthy eating)</li>
<li>Healthy eating</li>
<li>A good marriage</li>
<li>Favorable genetics</li>
<li>Higher income</li>
<li>Cancer avoidance</li>
<br/>
Gender-specific analysis required additional data cleaning and normalization. Results showed substantial overlap in top factors across genders, though some differences emerged: for men, “spending time with women” ranked #7, while for women, “having a dog” appeared in the top 10.

Key negative longevity factors were consistent across both genders, highlighting universal risks:
<li>Mental illness</li>
<li>Smoking</li>
<li>Obesity</li>
<li>Heavy alcohol use</li>

These four factors had the greatest negative impact, with others trailing significantly.
<br/><br/>

TECHNIQUES FOR CAPSTONE <br/>
Exploratory Data Analysis (EAD) and Visualize Results<br/>
Feature Engineering<br/>
Build a Simple Model<br/>
Fit and Train Multiple Models: linear regression, ridge, lasso, random forest, and gradient boosting<br/>
Compare and Choose the Best Model<br/>
Perform Hyperparameter Tuning Using GridSearchCV<br/>
Perform Optimization with Random Search<br/>
Visualize Results of Model Performance<br/>
<br/><br/>
SUMMARY OF FINDINGS<br/>
Among the five machine learning models evaluated, the Gradient Boosting achieved the best performance with the lowest test RMSE and highest R² score, indicating strong predictive accuracy and generalization. Random Forest Regressor was closely following Gradient Boosting in both metrics. The Linear, Lasso, and Ridge Regression models showed weak performance, likely due to excessive coefficient shrinkage and had minimal benefit from regularization. Overall, ensemble methods (Random Forest and Gradient Boosting) outperformed linear models, highlighting their effectiveness in capturing complex patterns in the data. Futher hypertuning of the best model improved its performance by almost 20%, which suggests that hypertuning is beneficial and may have a positive impact on model performance.Visualization charts are included to cleary show comparisons between the models. In conclusion, when and if I have new data in the future, I can use this model to make predictions to identify the longevity of the subject.
<br/>
<br/>
PERSONAL SUCCESS MEASURES <br/>
	1. Did I use data that I was interested in?
	2. Did this process answer my questions to help me further understanding of the topic?
	3. Did I further my understanding of Python programming, data science techniques, preparing data, building multiple machine learning models, plotting results?
	4. Did I further my understanding of data visualization techniques, using maplotlib and seaborn?
<br/><br/>
DATA SOURCE AND CITATION <br/>
• Arvidsson, Joakim. Longevity Factors (2023): URL: https://www.kaggle.com/datasets/joebeachcapital/life-longevity-factors