# Mission 4 — Machine Learning Task Types

## 1. Answer: What Tasks Can Machine Learning Perform?

Machine learning can solve different kinds of problems. The task type depends on the output we want, the available data and the objective of the system.

Four important task types are classification, regression, clustering and generation.

### A. Classification

Classification predicts a category or class.

**Example:** Predicting whether a battery is operating normally or has a fault.

Possible outputs are `Normal` and `Fault`.

### B. Regression

Regression predicts a numerical value.

**Example:** Estimating the power consumption of a chip from its design characteristics.

The output could be a numerical value such as `2.4 W`. This is an illustrative example, not a measured result.

### C. Clustering

Clustering groups data points according to their similarities without requiring predefined class labels.

**Example:** Grouping battery operating records with similar voltage and temperature patterns to explore different operating conditions.

The resulting groups do not automatically represent confirmed fault categories; an engineer must interpret and validate them.

### D. Generation

Generation produces new content, such as text, images, audio or code.

**Example:** Generating a first draft of Verilog code from a natural-language description.

Generated code must be reviewed, compiled and tested before it is trusted.

## 2. Comparison Table

| Task type | Main output | Typical question | Engineering example |
|---|---|---|---|
| Classification | Category or class | Is the battery faulty? | Normal/fault classification |
| Regression | Numerical value | What power will the chip consume? | Power estimation |
| Clustering | Groups of similar records | Which records behave similarly? | Exploring battery operating patterns |
| Generation | New content | Can a code draft be produced from this specification? | Verilog code generation |

## 3. Why the Distinction Matters

The task type determines how a system's output should be interpreted and evaluated.

- Classification results can be evaluated using measures such as accuracy, precision, recall and a confusion matrix.
- Regression results can be evaluated using measures such as mean absolute error (MAE) or root mean squared error (RMSE).
- Clustering can be evaluated using suitable clustering metrics and domain knowledge; the groups may not have an objectively correct label.
- Generation requires checks for correctness, relevance, completeness and compliance with the specification.

Some applications combine multiple task types. For example, a system may classify a fault and then generate a written explanation. Therefore, classification should focus on the primary task being discussed.

## 4. Evidence and Verification

Sources to consult:

1. Google for Developers — Introduction to Machine Learning: https://developers.google.com/machine-learning/intro-to-ml
2. IBM — What is Machine Learning?: https://www.ibm.com/think/topics/machine-learning

These are starting points for the basic ML concepts. Before submission, I will check that the references support the specific definitions and evaluation methods used here and add a more specialised source if necessary.

## 5. Reflection

I learned that classification predicts categories, regression predicts numerical values, clustering discovers groups of similar data, and generation creates new content. These tasks have different outputs, so they require different evaluation methods. In engineering, a plausible prediction or generated code is not sufficient by itself; the result must be checked against measurements, specifications or tests.

