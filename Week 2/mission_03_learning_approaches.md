# Mission 3 — Learning Approaches

## 1. Answer: How Do Machines Learn?

Machine learning has different approaches depending on the type of data available and how the system receives feedback. Four important approaches are supervised learning, unsupervised learning, reinforcement learning and self-supervised learning.

### A. Supervised Learning

Supervised learning uses labelled examples. Each training example contains input features and a known target. The model learns a relationship between the inputs and the target.

**Example:** Predicting whether an email is spam using previously labelled emails.

### B. Unsupervised Learning

Unsupervised learning works with data that does not have supplied target labels. It can identify patterns, similarities or groups in the data.

**Example:** Grouping similar customer records into clusters without predefined group labels.

### C. Reinforcement Learning

Reinforcement learning involves an agent interacting with an environment and receiving rewards or penalties. The agent learns a policy for choosing actions to maximise cumulative reward.

**Example:** An agent learning to navigate a simulated environment by receiving rewards for reaching a destination.

### D. Self-Supervised Learning

Self-supervised learning creates training targets from the data itself. The model learns useful patterns without requiring a separate human-provided label for every training example.

**Example:** A language model learning to predict missing or next tokens from text.

## 2. Comparison Table

| Approach | Training signal | Main purpose | Example |
|---|---|---|---|
| Supervised learning | Labelled input-output examples | Predict a known target | Spam classification |
| Unsupervised learning | Data without supplied target labels | Discover patterns or groups | Customer clustering |
| Reinforcement learning | Rewards from interaction | Learn actions or a policy | Simulated robot navigation |
| Self-supervised learning | Targets generated from the data | Learn representations or predict parts of data | Next-token prediction in text |

## 3. Engineering Example

Imagine an engineer wants to analyse temperature and voltage readings from a battery pack.

- **Supervised learning:** Use historical measurements labelled as normal or faulty to train a fault classifier.
- **Unsupervised learning:** Group operating records by similarity to explore different operating patterns.
- **Reinforcement learning:** In a carefully controlled simulation, train an agent to select actions that optimise a defined battery-management objective.
- **Self-supervised learning:** Learn patterns from large amounts of unlabelled sensor time-series data by predicting masked or future readings.

These are illustrative applications. Whether a particular approach is suitable depends on the available data, objective, safety constraints and evaluation method.

## 4. Evidence and Verification

Sources to consult:

1. Google for Developers — Introduction to Machine Learning: https://developers.google.com/machine-learning/intro-to-ml
2. IBM — What is Machine Learning?: https://www.ibm.com/think/topics/machine-learning

I will consult these references and check whether they support the distinctions made above. If a source does not explain a particular learning approach, I will locate an additional reliable reference rather than treating the claim as verified.

## 5. Reflection

I learned that machine learning is not a single training method. Supervised learning uses labelled examples, unsupervised learning explores data without supplied target labels, reinforcement learning uses rewards from interaction, and self-supervised learning generates learning targets from the data itself. The approach should be selected according to the problem, available data and required outcome.

