# UC_Berkeley_Module20.1_Exploratory_Data_Analysis
Author: Kelly Lieu <br/>

BACKGROUND <br/>
My goal is for this capstone is to learn and practice how to apply ML/AI techniques with data visualization tools. It was important to me to choose a dataset that was easy to obtain and a topic that I can learn from to apply at home or at work. The data comes from Kaggle called, "Longevity Factors." 
<br/><br/>
WE WILL EXPLORE <br/>
What longevity factors provide most gain in years of life?
What factors provide the most gain in years of life for females?
What are the top features based on the weighted impact of strength of science on years?
How do the stronger science features rank against the suggestive features?
What other insights can I derive from the data?
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
FEATURE ENGINEERING<br/>
The next sequence of steps is to perform feature engineering to prepare my dataset for building a model. Below I will start with a copy of the previous dataframe and perform the following:
<li>Identify categorical variables</li>
<li>Use one-hot encoder on categorical features</li>
<li>Create interaction terms (multiply factor and strength of science)</li>
<li>Create polynomial features and create a dataframe (except target col)</li>
<li>Create combined original dataframe with polynomial dataframe</li>
<li>Use StandardScaler to scale all my features (except target col)</li>
<li>Add back target column and I am ready to build my model</li>
<br/>
TECHNIQUES FOR CAPSTONE <br/>
Exploratory Data Analysis (EAD) and Visualize Results
Feature Engineering
Fit and Train Multiple Models
Compare Models Using GridSearchCV
Choose the Best Model
Perform Hyperparameter Tuning
Choose the Best Features
Visualize Results of Predictive Analysis
<br/><br/>
PERSONAL SUCCESS MEASURES <br/>
	1. Did I use data that I was interested in?
	2. Did my model answer my questions to help me further understanding of the topic?
	3. Did I further my understanding of data science techniques, cleansing data, filtering data, calculating data, plotting data?
	4. Did I further my understanding of storytelling with data visualization techniques, using maplotlib style fivethirtyeight?
<br/><br/>
DATA SOURCE AND CITATION <br/>
• Arvidsson, Joakim. Longevity Factors (2023): URL: https://www.kaggle.com/datasets/joebeachcapital/life-longevity-factors