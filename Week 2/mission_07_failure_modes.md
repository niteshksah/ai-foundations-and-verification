# Mission 7: Machine Learning Failure Modes

## 1. Objective

Understand why machine learning models can fail, identify common failure modes, and learn how to reduce their impact in engineering applications.

## 2. Failure Mode 1: Poor-Quality Data

### Description

A machine learning model learns patterns from its training data. If the data contains incorrect values, missing measurements, inconsistent units, or incorrect labels, the model may learn misleading patterns.

### Example: Battery Monitoring

Suppose a battery monitoring model is trained using temperature readings from a faulty sensor. It may learn an incorrect relationship between temperature and battery condition.

### Possible Solutions

- Check for missing and invalid values.
- Verify sensor calibration.
- Use consistent measurement units.
- Review incorrect or uncertain labels.
- Collect representative data from the intended operating conditions.

## 3. Failure Mode 2: Overfitting

### Description

Overfitting occurs when a model learns the training examples too closely, including noise and accidental patterns. As a result, it may perform poorly on unseen data.

### Example: Semiconductor Manufacturing

Suppose a model learns to classify defective semiconductor wafers using a small dataset. It might memorise patterns specific to those training samples rather than learning features that generalise to new wafers.

### Possible Solutions

- Use separate training, validation, and test datasets.
- Collect more representative training examples.
- Use regularisation or a simpler model where appropriate.
- Compare training performance with validation performance.
- Avoid repeatedly tuning the model against the test set.

## 4. Failure Mode 3: Distribution Shift

### Description

Distribution shift occurs when the data encountered after deployment differs from the data used during training. The model's performance may decrease because previously learned patterns no longer represent the current conditions.

### Example: Industrial Temperature Prediction

Suppose a model is trained using measurements from one operating environment. If the equipment later operates at different temperatures or loads, the model may produce less accurate predictions.

### Possible Solutions

- Monitor model performance after deployment.
- Collect data from different operating conditions.
- Test the model on representative scenarios.
- Retrain or update the model when justified by new evidence.
- Provide a fallback procedure when predictions are unreliable.

## 5. Comparison of the Three Failure Modes

| Failure mode | Main cause | Possible consequence | Prevention or mitigation |
|---|---|---|---|
| Poor-quality data | Incorrect, missing, or inconsistent data | Misleading learned patterns | Data validation and cleaning |
| Overfitting | Learning training data too closely | Poor performance on unseen data | Validation, regularisation, and suitable model complexity |
| Distribution shift | Real-world data changes | Decreased performance after deployment | Monitoring and representative new data |

## 6. Engineering Safety Considerations

Machine learning predictions should not automatically be treated as correct. In safety-critical applications, such as battery management or semiconductor manufacturing, engineers should:

- Define acceptable error limits.
- Test the model under relevant operating conditions.
- Consider the consequences of false positives and false negatives.
- Monitor performance after deployment.
- Use appropriate protective mechanisms and human review where necessary.

## 7. Verification Checklist

- [ ] I can explain each of the three failure modes.
- [ ] I can distinguish data-quality problems from overfitting.
- [ ] I can explain how distribution shift affects deployed models.
- [ ] I have identified at least one mitigation for each failure mode.
- [ ] I have checked the definitions against credible references.

## 8. Sources to Consult

1. Google Machine Learning Crash Course: https://developers.google.com/machine-learning/crash-course/
2. Google Machine Learning Glossary: https://developers.google.com/machine-learning/glossary

Consult the references and verify the relevant definitions before marking the claims as verified.

## 9. Reflection

**What I learned:**  
I learned that machine learning models can fail because of poor-quality data, overfitting, or changes in real-world conditions.

**What surprised me:**  
A model can perform well during testing but still become unreliable after deployment if the operating environment changes.

**How I will apply this:**  
In an engineering project, I will check data quality, evaluate the model on unseen examples, and consider how its performance could change under different operating conditions.

**Limitation:**  
The engineering examples in this document are illustrative scenarios, not reports of verified incidents or measured experimental results.
