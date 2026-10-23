# Mission 5 — Anatomy of an ML Model

## 1. Answer: How Does a Machine Learning Model Work?

A machine learning model is a system that uses learned patterns to produce predictions or outputs from input data. An algorithm describes the method used to learn those patterns, while a trained model contains the learned parameters produced by training.

### Important Terms

**Algorithm:** A procedure or method used to train a model. For example, gradient descent can adjust model parameters to reduce a loss function.

**Model:** The learned system that takes input data and produces an output.

**Training:** The process of using training data to learn model parameters.

**Inference:** Using a trained model to produce a prediction or output for new input data.

**Parameters:** Values learned during training, such as weights and biases in a neural network.

**Hyperparameters:** Configuration choices that control training or model design, such as the learning rate or number of hidden layers.

**Loss function:** A function that measures how far a model's prediction is from the desired result during training.

## 2. The ML Workflow

```text
Define the problem
        |
        v
Collect and prepare data
        |
        v
Choose a model and algorithm
        |
        v
Train the model
        |
        v
Learn model parameters
        |
        v
Evaluate the model
        |
        v
Use the trained model for inference
        |
        v
Monitor results and improve when needed
```

This is a simplified workflow. In practice, evaluation may reveal problems that require changes to the data, features, model or training process.

## 3. Engineering Example: Predicting Chip Power

Imagine an engineer wants to estimate a chip's power consumption from design-related inputs.

1. **Problem:** Estimate power consumption for a given design.
2. **Data:** Gather suitable historical design measurements and corresponding power values.
3. **Features:** Select relevant inputs, such as operating frequency and activity estimates, when available.
4. **Algorithm:** Select a suitable regression algorithm.
5. **Training:** Use training examples to learn model parameters.
6. **Evaluation:** Compare predictions with known power values from data kept separate from training.
7. **Inference:** Supply information about a new design and obtain an estimated power value.
8. **Review:** Compare the estimate with appropriate engineering analysis or measurements before relying on it.

This is an illustrative workflow, not a completed experiment or a claim that a specific model was trained.

## 4. Parameters vs. Hyperparameters

| Parameters | Hyperparameters |
|---|---|
| Learned from data during training | Set or selected to control model design or training |
| Examples: neural-network weights and biases | Examples: learning rate and number of hidden layers |
| Their values change as training updates the model | Usually configured before or between training runs |

Hyperparameters can be tuned by comparing candidate models. A selected hyperparameter configuration is not itself proof that a model will perform well on unseen data.

## 5. Evidence and Verification

Google for Developers provides learning material on model training, regression, neural networks and model evaluation.

Sources:

1. Google for Developers — Machine Learning Crash Course: https://developers.google.com/machine-learning/crash-course/
2. Google for Developers — Machine Learning Glossary: https://developers.google.com/machine-learning/glossary

I will consult these references to check the meanings of training, inference, parameters and hyperparameters. I will distinguish source-supported definitions from the illustrative chip-power example.

## 6. Reflection

I learned that an algorithm is the method used to learn, a trained model contains learned parameters, training develops those parameters from data, and inference uses the resulting model to produce outputs. I also learned that parameters and hyperparameters have different roles. In engineering, a model's output should be evaluated and checked before it is used to support an important decision.

