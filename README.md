# Heart Disease Classification

Coronary heart disease is a chronic disease of the heart with a narrowing of the coronary arteries. This can lead to disturbed blood flow of the heart muscle. Complications such as a myocardial infarction, heart insufficiency and cardiac arrythmias are possible consequences. Coronary heart disease is the leading common cause of death in Germany and around the world and leads to high costs in the health system (Busch, Kuhnert 2017). Several risk factors such as smoking, high blood pressure, diabetes and high cholesterol levels, among others, play a role in causing the disease. It can be diagnosed by means of invasive and non-invasive techniques.

The aim of the project is to predict the occurence of coronary heart disease in patients by building a classification model.

A possible use case would be screening for and identifying high-risk patients. The target audience who the project is aimed for could be general practioners and cardiologists. They would need to perform cardiac examinations and the results would be fed into the algorithm.
A first screening could be performed on cheaper parameters, such as age, cholesterol levels, blood pressure, blood sugar and a resting ECG in order to avoid examinations in healthy patients with low risk. If the patient is screened / classified positive by the algorithm for heart disease, the following consequences could be drawn in an attempt to reduce risk of complications such as a myocardial infarction: prescribing or changing medication, regular check-ups, reducing risk factors or peforming coronary angiography with possible stent implantation. Apart from the ethical perspective of preventing or reducing the risk of disease, this use case could also be of interest for health insurance companies regarding cost-effectiveness: Would it be more cost-efficient to pay extra cardiac examinations for screening than paying for rehabilitation and disability if the screening is not performed?

The dataset originates from the UCI Machine Learning Repository: Heart Disease Data Set, July 1988 (http://archive.ics.uci.edu/ml/datasets/Heart+Disease).

A number of classification models were built in Python. A k-Nearest-Neighbors model yielded the best results with an accuracy of 85% and sensitivity of 88%.

<br>

**Contents of the notebook:**
- Introduction
- Reading in dataset
- Data structure (Univariate Analysis)
    - Histograms
    - Box plots metric variables
    - Insights of the univariate analysis
- Splitting data into training and test set
<br>

- Exploratory Data Analysis (Bivariate Analysis)
    - Relationship between predictors and outcome
        - Categorical predictors and outcome
            - Proportions plot
            - Chi-Squared tests
        - Numeric predictors and outcome
            - Box plots, Proportions plot
            - Test statistic for metric independent variables (Shapiro-Wilk for normal distribution, subsequently Mann-Whitney-U for group comparison)
    - Relationship between predictors
        - Chi-squared test among categorical predictors
        - Correlations between metric predictors
        - Relationship between metric and categorical predictors
    - further possible questions
            - Are women with myocardial infarction more frequently asymptomatic than men?
            - Do elevated blood pressure, blood sugar and cholesterol occur together more often?
<br>

- Preprocessing
    - Data Cleaning
        - Missing values
        - Inconsistent values
    - Data Transformation
        - Scaling
        - Encoding of remaining categorical variables
<br>

- Model Training
- Model Evaluation
    - Data preprocessing for test set
    - Evaluation on the test set and metrics
<br>

- Limitations
- Conclusion
- Bibliography

