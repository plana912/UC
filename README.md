### Capstone Project - Classification Machine Learning Modeling for Hypertension Indicators

**Author: Paul Jibrail**

#### Executive summary
This capstone project's objective is to utilize machine learning models to classify patients for hypertension with high accuracy based on 13 data points, most of which are results from medical tests or service results.  These models can be utilized as a validation method or cross-checking by medical personnel when working with current patients.  Especially, in cases where the initial medical services focus is not necessarily hypertension and a machine learning model can assist in proactive care and validating current care circumstances.  To accomplish this several machine learning models will be trained and tested with a high performance objective for predicting hypertension in patients.  Though regardless of the models' performance they can and will not be the sole means for hypertension determination in patients.

#### Rationale
Predicating hypertension in patients with various indicators can be of great value for applying care more proactively and even for validating the current care services. Using a machine model will also improve quality control to ensure patient circumstances are not accidently missed impacting care delivery quality.

#### Research Question
Can a machine learning model predict with high accuracy whether patients have hypertension based on several relevant medical indicators, e.g., ECG results? Then using the resulting machine model selected to supplement care providers work.

#### Data Sources
The data set I have selected for this project is from Kaggle. The title is: "Diabetes, Hypertension and Stroke Prediction"  which has three separate data sets within it, one of which is hypertension_data.csv.  It is partially cleaned data. The poster of the data was Prosper Chuks. He based the data posting on CDC data (BRFSS 2015).  The data set is 1.09 MB with 14 features and 26,083 samples. License CC0: Public Domain

[Hypertension Data](https://www.kaggle.com/datasets/prosperchuks/health-dataset?select=hypertension_data.csv)

#### Methodology
1. Clean data of incomplete data samples
2. Reviewed data set for oridinal or nominal categorical feature changes
3. Balancing of data based on class distribution (0,1); utilizing data over sampling function to add data samples to balance classes
4. Relabel data features to make more readable for data modeling work
5. Split data in four subsets (X_train, y_train, X_test, y_test)
6. Select machine classification models for fitting and testing; KNN Classifier, Support Vector Machine (SVM), Decision Tree, Random Forest
7. Evaluate the models with several hyper-parameters, accuracy metrics, and cross-validation functions
8. Determine the most impactful features that indicate hypertension
9. Interpret the models performance in alignment with the project's objective(s)
10. Identify the best model(s) to apply for medical services providers to apply
11. Document top impacting features and state impact in non-data scientist terminology
12. Document business oriented insights and actionable recommendations
13. Provide an example of simple deployment packaging for non data scientist to use (joblib pkl)

#### Results
That all machine models produced high accuracy / performance in their predictions. Several techniques were utilized to ensure the results were not due to overfitting. Of the 14 indicators represented by data set features, these were the 'Top 5' indicators that most of the models' classification performance were due to:
1. st_depressed (ST ECG Depression)
2. art_color (arterial flourosopy imaging color)
3. chest_pain (chest pain)
4. max_hr (maximum heart rate)
5. chol (cholesterol level)
   
See the companion Jupyter Notebook for more information on each term/feature listed.

I selected the KNN Model even a couple other models did well too. The KNN model also executes fast.

All Business Insights and Actionable Recommendation are at the end of the Juypter Notebook.

Business Results
[Interesting Findings](https://github.com/plana912/UC/blob/main/data/InterestingFindings.jpg)

[Actionable Insights](https://github.com/plana912/UC/blob/main/data/ActionableInsights.jpg)

#### Next steps
Utilize the machine learning models in proactive services delivery, quality assurance, and governnce activities at medical service providers. Further, gather data to train and improve the models. See the Conclusion / Findings section of the Juypter Notebook for details.

#### Outline of project

Jupyter Notebook link: [Paul Jibrail Capstone 24.1 Oct 2024](https://github.com/plana912/UC/blob/main/Paul%20Jibrail%20Capstone%2024.1%20Oct%202024.ipynb)

File Name: Paul Jibrail Capstone 24.1 Oct 2024.ipynb

Outline:
- Business Understanding & Objectives
- Data
- Exploratory Data Analysis (EDA)
- Data Preparation
- Modeling
- Conclusion / Findings
- Deployment / Implementation [Test_PKL_File notebook](https://github.com/plana912/UC/blob/main/Test_PKL_File.ipynb)

##### Contact and Further Information
Paul Jibrail
Mollitiam Solutions LLC
paul.jibrail@molltiamsolutions.com
