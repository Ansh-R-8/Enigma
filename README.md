# Loan Default Prediction Model for Fairness and Accuracy

## Overview

This project addresses a critical challenge in the financial sector: credit default prediction. It emphasizes building a model that is not only accurate in predicting loan defaults but also fair and unbiased in its outcomes, particularly concerning gender. This was achieved through innovative techniques, specifically using XGBoost and Fairlearn's ThresholdOptimizer to minimize gender bias in the model's predictions. The project's success was recognized by its 1st place win at the Enigma Hackathon, held within Codefest'24 at IIT BHU.

## Model Used

- **XGBoost**: A powerful gradient boosting algorithm known for its effectiveness in credit risk prediction tasks.

## Key Points

### Fairness Integration

- **Fairlearn's ThresholdOptimizer**: Ensures demographic parity for gender during model training. This helps mitigate potential bias in the model's predictions and prevent discriminatory outcomes based on gender.

### Hyperparameter Tuning

- **Hyperopt**: Utilized for hyperparameter tuning with Stratified K-Fold Cross-Validation. This process optimizes the model's performance while maintaining fairness.

### Preprocessing and Evaluation

- **Data Preprocessing**: The code incorporates steps like handling missing values and encoding categorical features.
- **Evaluation Metrics**: The model's performance is evaluated using metrics such as F1-score and Demographic Parity Ratio (DPR) for gender.

## Results

The script outputs the following key results to assess the model's performance and fairness:

- **F1-score**: 0.5342. This metric indicates a good balance between precision and recall in predicting loan defaults.
- **Demographic Parity Ratio (DPR) for Gender**: 0.9799. This value close to 1 signifies a high level of fairness achieved by the model. In simpler terms, the model predicts loan defaults at similar rates for both genders, mitigating potential gender bias.

## Conclusion

By integrating fairness into the loan default prediction model, this project showcases the potential for creating more equitable financial tools. The recognition received at the Enigma Hackathon underscores the importance and effectiveness of addressing bias in machine learning models.

## Submission File

The predictions of the model are stored [here](./submission_Enigma.csv)
