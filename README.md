### **Page available at: https://faisaljina.github.io/machine-learning-ou/**
#

# Machine Learning on student records in Python

This uses the Open University Learning Analytics dataset package, available from the Knowledge Media institute, The Open University.
The seven large datasets (raw data not included in repo due to size) on Open University students were used with a goal of predicting who may fail or withdraw from their university course. 
The datasets consist of:
1. A list of available modules and their details.
2. Information about assessments in module-presentations. Usually, every presentation has a number of assessments followed by the final exam.
3. Information about the available materials in the Virtual Learning Environment (VLE). Typically, these are html pages, pdf files, etc. Students have access to these materials online and their interactions with the materials are recorded.
4. Demographic information about the students together with their results.
5. Information about the time when the student registered for the module presentation. For students who unregistered the date of unregistration is also recorded.
6. Results of students’ assessments. If the student does not submit the assessment, no result is recorded. The final exam submissions is missing if the result of the assessments is not stored in the system.
7. Information about each student’s interactions with the materials in the VLE.  

This project uses Python (as a Jupyter notebook) and both classification and regression methodologies to predict which students are suspected to fail or withdraw from a module. Naturally, this involved extensive use of the `sklearn` and `imblearn` packages.

### Features
- EDA
- Feature Engineering
- Pipelines
- Feature Importance
- Visualisation

### Techniques
- SMOTE
- PowerTransformer
- KNNImputer
- Gradient Boosting
- ElasticNet
- Ridge/Lasso Regression

## Summary
1. The datasets were explored, merged, and features engineered using summary statistics and charts.
2. The merged dataset was cleaned, reduced to eliminate extraneous information, and outliers were addressed.
3. Encoding of variables and colinearity was examined.
4. The dataset was split into test and train sets, transformed, missing values imputed, and the minority target class oversampled to generate synthetic data.
5. Pipelines were built for both classification and regression approaches.
6. Classification used recall score and confusion matrices as metrics, GridSeachCV and RandomizedSearchCV for model selection, and the best model was confirmed statistically.
7. Feature importance was visualised for both approaches, and outcomes for the university were derived.
