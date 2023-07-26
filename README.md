## Fraudulent Firm Classification Project

### Background

In this project, I collected exhaustive one-year non-confidential data from the Auditor Office of India for the years 2015 to 2016. The objective is to build a classification model that can predict suspicious firms based on present and historical risk factors. The auditors require this model to identify potentially fraudulent firms, thus aiding in their investigative processes and ensuring the integrity of the financial ecosystem.

### Dataset Characteristics

- Multivariate dataset
- Subject Area: Other
- Associated Task: Classification
- Attribute Type: Real
- Number of Instances: 777
- Number of Attributes: 18
- Missing Values: Yes

### Attribute Information

The dataset contains various risk factors from different areas, such as past records of the audit office, audit-paras, environmental conditions reports, firm reputation summaries, ongoing issues reports, profit-value records, loss-value records, follow-up reports, etc. These risk factors have been evaluated based on their probability of existence derived from present and past records.

The sectors and the corresponding counts of firms in the dataset are as follows:

- Irrigation: 114 firms
- Public Health: 77 firms
- Buildings and Roads: 82 firms
- Forest: 70 firms
- Corporate: 47 firms
- Animal Husbandry: 95 firms
- Communication: 1 firm
- Electrical: 4 firms
- Land: 5 firms
- Science and Technology: 3 firms
- Tourism: 1 firm
- Fisheries: 41 firms
- Industries: 37 firms
- Agriculture: 200 firms

### Project Overview

1. Data Loading and Exploration:
   - Loaded the dataset using pandas and visualized the first five samples.
   - Checked the shape and column names of the data frame.
   - Handled missing values by replacing them with the mean value of the "Money_Value" column.

2. Data Preprocessing:
   - Created the feature set (X) and target variable (Y) by dropping unnecessary columns.
   - Split the data into training and testing sets using a fixed random state.
   - Standardized the features using the StandardScaler.

3. Model Building and Evaluation:
   - Built a Support Vector Machine (SVM) classification model with customized hyperparameters.
   - Evaluated the model's accuracy, precision, recall, specificity, and classification error.
   - Plotted the ROC curve and calculated the ROC AUC score.
   - Calculated the cross-validated ROC AUC score to validate the model's performance.

### Conclusion

The developed classification model can assist auditors in identifying suspicious firms by predicting potential fraudulent activities. The high accuracy, precision, recall, and ROC AUC score indicate the model's effectiveness in distinguishing between fraudulent and non-fraudulent firms. As a result, this predictive model can significantly enhance the efficiency and effectiveness of auditing processes, contributing to a more secure and trustworthy financial environment.

Please feel free to explore the Jupyter Notebook files provided in this repository to gain insights into the data exploration, preprocessing, and model building steps. Your valuable feedback and suggestions are always welcome!
