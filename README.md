# Early Detection of Alzheimer's Disease using Machine Learning

## Project Overview

This project explores the application of machine learning techniques to detect Alzheimer's disease using MRI scan data. The primary objective is to evaluate different algorithms' effectiveness and improve diagnostic accuracy. The results of this study show promising directions for future research in automated Alzheimer's detection.

## Abstract

The project applies machine learning techniques to detect Alzheimer's disease through MRI scan data. The study evaluates various algorithms to improve diagnostic accuracy, aiming to develop a reliable, automated tool for early Alzheimer's detection.

## Introduction

Alzheimer's disease (AD) is a progressive neurodegenerative disorder impacting cognitive function, memory, and behavior. Early detection is crucial for effective management and treatment. This study aims to enhance early detection using machine learning to analyze MRI data, potentially offering a more objective and consistent diagnostic approach compared to traditional methods.

## Dataset and Features

- **Dataset**: OASIS-2 dataset, provided by Washington University in St. Louis.
- **Subjects**: 150 subjects aged 60 to 96, with MRI scans and associated clinical data.
- **Features**:
  - EDUC: Years of Education
  - SES: Socioeconomic Status
  - MMSE: Mini Mental State Examination
  - CDR: Clinical Dementia Rating
  - eTIV: Estimated Total Intracranial Volume
  - nWBV: Normalize Whole Brain Volume
  - ASF: Atlas Scaling Factor

## Methodology

### Preprocessing Steps

- Removing duplicates
- Handling null values (imputation for SES and MMSE columns)
- Group label adjustment (unifying dementia-related labels)
- Visit selection (using only the first visit data)
- Label encoding (binary encoding for Group and gender columns)
- Dropping irrelevant columns
- Outlier removal
- Feature and target separation
- Standardization of feature data

### Machine Learning Models

1. **Logistic Regression**
   - Hyperparameter tuning using Grid Search with Cross-Validation
   - Regularization strength and penalty types

2. **Random Forest**
   - Hyperparameter tuning using GridSearchCV
   - Parameters: n_estimators, max_depth, min_samples_split

3. **Support Vector Machine (SVM)**
   - Hyperparameter tuning using Grid Search with Cross-Validation
   - Kernel type, regularization parameter, and kernel coefficient

4. **Decision Tree**
   - Hyperparameter tuning using Grid Search with Cross-Validation
   - Criterion and max depth

## Evaluation Metrics

- **Accuracy**: Ratio of correctly predicted observations to total observations
- **Precision**: Ratio of correctly predicted positive observations to total predicted positives
- **Recall (Sensitivity)**: Ratio of correctly predicted positive observations to all observations in the actual class
- **F1-Score**: Weighted average of Precision and Recall
- **Confusion Matrix**: Performance table showing true positive, true negative, false positive, and false negative counts

## Results and Discussion

The experiments' results indicate that different machine learning models offer varying levels of accuracy in detecting Alzheimer's disease. The performance metrics guide the selection of the most effective model for this task.

## Conclusion

The study demonstrates that machine learning techniques can significantly contribute to the early detection of Alzheimer's disease. Future research could focus on refining these models and exploring additional datasets to enhance diagnostic accuracy further.

## Acknowledgments

We acknowledge the support from Cairo University and the availability of the OASIS-2 dataset from Washington University in St. Louis.

## Contact Information

For further information, please contact the authors via their provided email addresses.
