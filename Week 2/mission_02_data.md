# Mission 2 — Understanding Data

## 1. Answer: What Is Data in Machine Learning?

Machine Learning (ML) uses data to identify patterns and make predictions or decisions. Understanding the data is important because incomplete, inaccurate or biased data can lead to unreliable results.

The main terms are:

- **Dataset:** A collection of examples used for analysis or machine learning.
- **Sample:** One individual example or record in a dataset.
- **Feature:** An input variable used by a model to make a prediction.
- **Label:** The known answer or category associated with an example in a labelled dataset.
- **Target:** The outcome that the model is intended to predict. In supervised learning, the target is usually represented by the label or target value in the training data.

## 2. Example Dataset: Predicting Fan Status

Consider a simple illustrative dataset for a temperature-controlled fan. The target is whether the fan should be ON or OFF.

| Sample | Temperature (°C) | Humidity (%) | Fan Status |
|---|---:|---:|---|
| 1 | 22 | 40 | OFF |
| 2 | 25 | 45 | OFF |
| 3 | 29 | 50 | OFF |
| 4 | 32 | 55 | ON |
| 5 | 35 | 60 | ON |
| 6 | 38 | 65 | ON |

**Important:** These are illustrative example values, not measurements from a real experiment.

### Identify the data components

- **Dataset:** All six rows in the table.
- **Sample:** Each individual row, such as Sample 4.
- **Features:** Temperature and humidity.
- **Label/target:** Fan Status.
- **Task:** Predicting whether the fan should be ON or OFF is a classification task because the output belongs to one of two categories.

This example illustrates a possible dataset. The rows alone do not prove that temperature and humidity cause the fan status, nor do they establish how a real fan controller operates.

## 3. Why Data Quality Matters

A model depends on the quality and relevance of the data used to develop and evaluate it.

1. **Incorrect values:** A faulty temperature sensor may record 80°C when the actual temperature is 30°C.
2. **Missing values:** Some records may not contain humidity measurements.
3. **Unrepresentative data:** Data collected only in one environment may not represent other operating conditions.
4. **Inconsistent units:** Mixing Celsius and Fahrenheit without conversion can confuse data analysis.
5. **Incorrect labels:** If a record says the fan was ON when it was actually OFF, the model may learn from a wrong answer.
6. **Biased data:** If important situations are underrepresented, model performance may be poor in those situations.

Before using a dataset, inspect its units, missing values, measurement accuracy, labels and relevance to the intended application.

## 4. Evidence and Verification

This document uses a six-row illustrative dataset to demonstrate the meanings of dataset, sample, feature, label and target. The values are examples created for learning; they are not external experimental evidence.

Research sources to consult:

1. Google for Developers — Introduction to Machine Learning: https://developers.google.com/machine-learning/intro-to-ml
2. IBM — What is Machine Learning?: https://www.ibm.com/think/topics/machine-learning

I will check these references for explanations of training data, features, labels and ML workflows before marking the concepts as independently verified.

## 5. Reflection

I learned that data is more than a collection of numbers. Each row represents a sample, the input columns represent features, and the desired outcome is the target. I also learned that incorrect sensor readings and labels can reduce the reliability of a model. In an engineering application, I should inspect data quality and understand how the data was collected before trusting a prediction.

