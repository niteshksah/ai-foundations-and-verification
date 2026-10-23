# Mission 6: Evaluating Machine Learning Models

## 1. Objective

Understand how to evaluate a machine learning model, check its performance on unseen data, and identify common evaluation mistakes.

## 2. Training, Validation, and Test Data

A dataset can be divided into three parts:

- **Training set:** Used to train the model and learn patterns.
- **Validation set:** Used to compare models and tune hyperparameters.
- **Test set:** Used for the final evaluation on data not used during training or model selection.

The test set should remain separate until the final evaluation.

## 3. Important Evaluation Concepts

### Generalisation

Generalisation is the ability of a model to perform well on new data that it has not seen during training.

### Overfitting

Overfitting occurs when a model learns the training data too closely, including noise or accidental patterns. It may perform well on training data but poorly on new data.

### Underfitting

Underfitting occurs when a model is too simple to learn the important patterns in the data.

### Data Leakage

Data leakage occurs when information that would not legitimately be available during training enters the model-building process. It can make evaluation results look better than real-world performance.

## 4. Common Evaluation Metrics

| Metric | Purpose |
|---|---|
| Accuracy | Measures the proportion of predictions that are correct. |
| Precision | Measures how many predicted positive cases are actually positive. |
| Recall | Measures how many actual positive cases the model identifies. |
| F1-score | Combines precision and recall using their harmonic mean. |
| MAE | Measures the average absolute difference between predicted and actual numerical values. |
| RMSE | Measures prediction error while penalising larger errors more strongly. |

The appropriate metric depends on the task and the consequences of incorrect predictions.

## 5. Example: Battery Fault Detection

Suppose a machine learning model identifies whether a battery cell has a fault.

- Training data is used to learn patterns associated with faults.
- Validation data helps select the model and tune its settings.
- Test data estimates performance on unseen examples.
- Recall is important when missing a genuine fault could create a safety risk.
- Precision is also important because excessive false alarms can lead to unnecessary inspections.

A high accuracy score alone does not guarantee that a battery fault detection model is safe or reliable.

## 6. Verification Checklist

- [ ] The training, validation, and test sets are clearly distinguished.
- [ ] The test set is not used to tune the model.
- [ ] Evaluation data represents the intended real-world use.
- [ ] Appropriate metrics are selected for the problem.
- [ ] Possible data leakage is checked.
- [ ] Results are reported honestly, including limitations.

## 7. Sources to Consult

1. Google Machine Learning Crash Course: https://developers.google.com/machine-learning/crash-course/
2. Google Machine Learning Glossary: https://developers.google.com/machine-learning/glossary

Consult these references and verify the definitions before marking the claims as verified in your learning log.

## 8. Reflection

**What I learned:**  
I learned that evaluating a machine learning model involves more than checking its accuracy. Separate datasets help estimate how well it performs on unseen data, while suitable metrics help explain different types of prediction errors.

**What I still need to understand:**  
I need more practice choosing evaluation metrics for different classification and regression problems.

**How I will apply this:**  
For an engineering project, I will evaluate a model using data that was not used for training and consider the consequences of false predictions before deciding whether its performance is acceptable.
