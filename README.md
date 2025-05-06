# Blood-Donation-Prediction-Predict Blood Donation

##Business Problem
Blood transfusion saves lives - from replacing lost blood during major surgery or a serious injury to treating various illnesses and blood disorders. Ensuring that there's enough blood in supply whenever needed is a serious challenge for the health professionals. According to WebMD," about 5 million Americans need a blood transfusion every year". Our dataset is from a mobile blood donation vehicle in Taiwan. The Blood Transfusion Service Center drives to different universities and collects blood as part of a blood drive. We want to predict whether or not a donor will give blood the next time the vehicle comes to campus in March 2007.

##Dataset Description
###Features:
1. Recency: Months since the last donation.
2. Frequency: Total number of donations.
3. Monetary: Total blood donated in c.c.
4. Time: Months since the first donation.

###Label:
Binary variable indicating whether the individual donated blood in March 2007 (Yes = 1, No = 0).

###Preprocessing Steps:
1. Normalization of values for consistent scaling.
2. Differentiation between features and labels.
3. Addressing class imbalance through oversampling techniques to improve model performance for the minority class (donors).

##Key Findings:
1. Dataset Structure and Cleaning
  o The dataset consists of columns with 576 values each, with no missing values or null entries.
  o All columns contain integer data types, simplifying preprocessing.
  o An irrelevant column, Unnamed: 0, containing only sequential numbers, was removed to optimize the analysis.
2. Challenges and Risks
  o Feature Scope: The dataset lacks demographic or behavioral data, which limits the predictive accuracy and generalizability of the analysis.
  o Biases: Uneven representation of donors poses a risk of skewed results, potentially impacting model performance and insights.
3. Next Steps
  o Conduct advanced feature engineering to improve dataset richness.
  o Implement methods to address data imbalance, such as resampling or using model techniques robust to biases.
  o Build models and evaluate their performance, ensuring appropriate metrics are used to account for dataset biases.

##Model Evaluation:
  Six machine learning models were trained, tested, and evaluated using accuracy and F1-scores for both classes (Class 0: Non-donors, Class 1: Donors).
  Analysis:
          Logistic Regression achieved the highest accuracy (78.61%) in the initial evaluation, followed by Random Forest and Naive Bayes (77.46% each).
          F1-scores for Class 1 (donors) were relatively low across models, indicating class imbalance challenges.
