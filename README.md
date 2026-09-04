Absolutely. Since your current work is specifically Deep Learning from Scratch → PyTorch → ANN → Customer Churn Prediction, your README should document what you have actually completed so far, without adding the upcoming experiments yet.

Copy this directly into your README.md:

# 🧠 Deep Learning From Scratch

A hands-on journey to understand **Deep Learning from the ground up** by learning the intuition, mathematics, and implementation behind neural networks before relying completely on high-level frameworks.

> **Understand → Derive → Implement → Experiment → Use Frameworks**

---

## 📌 About This Repository

This repository documents my journey of learning **Deep Learning from scratch**.

The goal is not only to use frameworks such as PyTorch, but to understand what happens inside a neural network during training.

The learning process focuses on:

- Understanding the intuition behind neural networks
- Understanding the mathematics
- Implementing core concepts from scratch
- Experimenting with different approaches
- Implementing neural networks using PyTorch
- Connecting theoretical concepts with real-world datasets

The journey started from a **single artificial neuron (Perceptron)** and has now progressed to building an **Artificial Neural Network (ANN) using PyTorch** for a real-world customer churn prediction problem.

---

# 🎯 Current Goals

The main objectives of this project are:

- Understand how artificial neurons work
- Understand weights and biases
- Understand weighted sums
- Understand activation functions
- Understand forward propagation
- Understand loss functions
- Understand backpropagation
- Understand the chain rule
- Understand gradients
- Understand gradient descent
- Understand learning rate
- Understand SGD and Mini-Batch SGD
- Understand optimization algorithms
- Build neural networks from scratch
- Understand ANN architecture
- Implement ANN using PyTorch
- Train a neural network on a real-world dataset
- Evaluate model performance
- Understand the complete Deep Learning training pipeline

---

# 🗺️ Learning Progress

```text
                DEEP LEARNING FROM SCRATCH
                           │
                           ▼
                      Perceptron
                           │
                           ▼
                    Weights & Bias
                           │
                           ▼
                     Weighted Sum
                           │
                           ▼
                 Activation Functions
                  ┌────────┼────────┐
                  ▼        ▼        ▼
               Sigmoid    Tanh     ReLU
                           │
                           ▼
                 Forward Propagation
                           │
                           ▼
                     Loss Function
                           │
                           ▼
                   Backpropagation
                           │
                           ▼
                      Chain Rule
                           │
                           ▼
                       Gradient
                           │
                           ▼
                  Gradient Descent
                           │
                           ▼
                    Learning Rate
                           │
                           ▼
                         SGD
                           │
                           ▼
                    Mini-Batch SGD
                           │
                           ▼
                     Optimizers
                           │
                           ▼
                    Multiple Neurons
                           │
                           ▼
                     Hidden Layers
                           │
                           ▼
             Artificial Neural Network
                           │
                           ▼
                         PyTorch
                           │
                           ▼
             Customer Churn Prediction
                           │
                           ▼
                    ANN Experiments
                           │
                           ▼
                 CNN → RNN → LSTM
                           │
                           ▼
                     Transformers
✅ Concepts Completed
1. Artificial Neuron

Studied the basic structure of an artificial neuron:

Inputs
  │
  ├── x₁ ── w₁ ──┐
  ├── x₂ ── w₂ ──┤
  ├── x₃ ── w₃ ──┤
  │              ▼
  │        Weighted Sum + Bias
  │              │
  │              ▼
  │       Activation Function
  │              │
  │              ▼
  │            Output

Mathematical representation:

z = w₁x₁ + w₂x₂ + ... + wₙxₙ + b

output = activation(z)
2. Weights and Bias

Learned the role of:

Weights
Bias
Weighted sum
Parameter learning

Weights determine how strongly each input influences a neuron.

Bias allows the neuron to shift its decision boundary.

3. Activation Functions

Studied the importance of activation functions and why neural networks need non-linearity.

Sigmoid
f(x) = 1 / (1 + e⁻ˣ)

Output range:

0 → 1

Useful for binary classification outputs.

Tanh
f(x) = tanh(x)

Output range:

-1 → 1
ReLU
f(x) = max(0, x)

ReLU is commonly used in hidden layers because it is simple and computationally efficient.

4. Forward Propagation

Learned how data moves through a neural network:

Input
  ↓
Weighted Sum
  ↓
Activation
  ↓
Hidden Layer
  ↓
Weighted Sum
  ↓
Activation
  ↓
Output

Forward propagation produces the model's prediction.

5. Loss Function

Learned that the loss function measures how different the model prediction is from the actual target.

Prediction
     │
     ▼
Loss Function
     │
     ▼
Error

The objective of training is to minimize this loss.

6. Backpropagation

Studied how neural networks calculate how much each parameter contributed to the error.

Backpropagation uses the chain rule to calculate gradients.

Loss
 ↓
Gradient
 ↓
Weights / Biases
7. Chain Rule

Studied the mathematical foundation behind backpropagation.

The chain rule allows gradients to be propagated backward through multiple operations and layers.

8. Gradient Descent

Learned how gradient descent updates model parameters.

Basic update equation:

new_weight = old_weight - learning_rate × gradient

The gradient tells us the direction of increasing loss.

Therefore, we move in the opposite direction to reduce the loss.

9. Learning Rate

Studied the importance of the learning rate.

Learning Rate
      │
      ▼
Size of parameter update
Too large
Overshooting
     ↓
Unstable training
Too small
Very slow learning

A suitable learning rate helps the model converge efficiently.

10. SGD

Studied Stochastic Gradient Descent.

Instead of calculating gradients using the entire dataset, SGD updates the parameters using individual training examples.

Advantages:

Faster updates
Lower memory requirement
Introduces useful randomness into training
11. Mini-Batch SGD

Studied Mini-Batch Gradient Descent.

Instead of using:

Entire Dataset

or:

One Sample

we use:

Small Batch

Example:

Dataset = 8000 samples

Batch size = 32

Training:

Batch 1 → Update
Batch 2 → Update
Batch 3 → Update
...

The variation between gradients from different batches is commonly referred to as gradient noise.

12. Optimization

Studied the role of optimizers in neural network training.

Initial optimizer concepts explored include:

Gradient Descent
SGD
Mini-Batch SGD
AdaGrad

The role of an optimizer is to update trainable parameters using gradients.

🧠 Neural Network Architecture

Progressed from a single neuron to multiple neurons and hidden layers.

Input Layer
     │
     ▼
Hidden Layer
     │
     ▼
Hidden Layer
     │
     ▼
Output Layer

This allows neural networks to learn increasingly complex relationships in data.

🚀 Current Project: Customer Churn Prediction

The current practical project is a Customer Churn Prediction ANN built using PyTorch.

The objective is to predict whether a customer will leave a company.

Dataset
Churn_Modelling.csv
Target
Exited

Where:

0 → Customer stays
1 → Customer exits
🔄 Data Preprocessing Pipeline

The current preprocessing pipeline is:

Raw Dataset
     │
     ▼
Remove unnecessary columns
     │
     ├── RowNumber
     ├── CustomerId
     └── Surname
     │
     ▼
Separate Features and Target
     │
     ▼
Encode Categorical Features
     │
     ▼
Train/Test Split
     │
     ▼
Feature Scaling
     │
     ▼
Convert to PyTorch Tensors
     │
     ▼
ANN
🧹 Data Cleaning

The following columns were removed:

RowNumber
CustomerId
Surname

These columns are not useful features for predicting customer churn.

🔤 Categorical Encoding

Categorical features such as:

Geography
Gender

were converted into numerical representations using one-hot encoding.

X = pd.get_dummies(
    X,
    columns=["Geography", "Gender"],
    drop_first=True
)
✂️ Train/Test Split

The dataset is divided into training and testing sets.

X_train, X_test, y_train, y_test = train_test_split(
    X,
    y,
    test_size=0.2,
    random_state=42,
    stratify=y
)

Current split:

80% → Training
20% → Testing

stratify=y is used to maintain a similar class distribution in both datasets.

📏 Feature Scaling

Features are standardized using StandardScaler.

scaler = StandardScaler()

X_train = scaler.fit_transform(X_train)
X_test = scaler.transform(X_test)

The scaler is fitted only on the training data to avoid data leakage.

🔢 PyTorch Tensors

The processed NumPy arrays are converted into PyTorch tensors.

X_train_tensor = torch.tensor(
    X_train,
    dtype=torch.float32
)

X_test_tensor = torch.tensor(
    X_test,
    dtype=torch.float32
)

y_train_tensor = torch.tensor(
    y_train,
    dtype=torch.float32
).reshape(-1, 1)

y_test_tensor = torch.tensor(
    y_test,
    dtype=torch.float32
).reshape(-1, 1)
🏗️ ANN Architecture

The current ANN architecture is:

Input Layer
    │
    │  11 features
    ▼
Linear Layer
11 → 16
    │
    ▼
ReLU
    │
    ▼
Linear Layer
16 → 8
    │
    ▼
ReLU
    │
    ▼
Linear Layer
8 → 1
    │
    ▼
Sigmoid
    │
    ▼
Churn Probability

In short:

11 → 16 → 8 → 1
💻 PyTorch Model
class ChurnANN(nn.Module):

    def __init__(self):
        super().__init__()

        self.layer1 = nn.Linear(11, 16)
        self.layer2 = nn.Linear(16, 8)
        self.output = nn.Linear(8, 1)

        self.relu = nn.ReLU()
        self.sigmoid = nn.Sigmoid()

    def forward(self, x):

        x = self.layer1(x)
        x = self.relu(x)

        x = self.layer2(x)
        x = self.relu(x)

        x = self.output(x)
        x = self.sigmoid(x)

        return x
📉 Loss Function

Binary Cross Entropy Loss is currently used:

criterion = nn.BCELoss()

This is appropriate for binary classification when the model outputs probabilities using a sigmoid function.

⚙️ Optimizer

The current optimizer is Adam:

optimizer = optim.Adam(
    model.parameters(),
    lr=0.001
)

Current learning rate:

0.001
🔥 Training

The ANN is currently trained for:

100 epochs

The training process follows:

Input Data
     ↓
Forward Propagation
     ↓
Prediction
     ↓
Calculate Loss
     ↓
Backpropagation
     ↓
Calculate Gradients
     ↓
Adam Optimizer
     ↓
Update Weights
     ↓
Repeat
📊 Training Loss

Training loss is recorded after every epoch.

loss_history = []

for epoch in range(epochs):

    predictions = model(X_train_tensor)

    loss = criterion(
        predictions,
        y_train_tensor
    )

    optimizer.zero_grad()

    loss.backward()

    optimizer.step()

    loss_history.append(loss.item())

The loss curve is plotted to observe the training process.

🧪 Model Evaluation

After training, the model is switched to evaluation mode:

model.eval()

Predictions are generated without calculating gradients:

with torch.no_grad():
    predictions = model(X_test_tensor)
🎯 Binary Classification

The model produces a probability between 0 and 1.

A threshold of 0.5 is used:

Probability >= 0.5
        ↓
      Churn

Probability < 0.5
        ↓
    No Churn

Implementation:

predicted_classes = (
    predictions >= 0.5
).float()
📈 Evaluation Metrics

The current model is evaluated using:

Accuracy

Measures the percentage of correctly classified customers.

accuracy = (
    predicted_classes == y_test_tensor
).float().mean()
Classification Report
print(
    classification_report(
        y_true,
        y_pred
    )
)

This provides:

Precision
Recall
F1-score
Support
📊 Confusion Matrix

A confusion matrix is used to understand the classification results.

                    Predicted
                  0          1

Actual  0       TN         FP

        1       FN         TP

Where:

TN = True Negative
FP = False Positive
FN = False Negative
TP = True Positive

The confusion matrix helps understand which types of predictions the model gets wrong.

🛠️ Technologies Used
Python
│
├── NumPy
├── Pandas
├── Matplotlib
│
├── Scikit-learn
│   ├── train_test_split
│   ├── StandardScaler
│   ├── accuracy_score
│   ├── classification_report
│   └── confusion_matrix
│
└── PyTorch
    ├── torch
    ├── torch.nn
    └── torch.optim
📂 Current Project Structure
deep-learning-from-scratch/
│
├── README.md
│
├── ANN/
│   └── ANN_Customer_Churn_PyTorch.ipynb
│
└── datasets/
    └── Churn_Modelling.csv

The exact folder structure may evolve as the project grows.

📚 Learning Philosophy

This repository follows a concept-first approach.

Instead of directly using:

model.fit(...)

the goal is to understand what happens internally:

Input
 ↓
Weights
 ↓
Weighted Sum
 ↓
Activation
 ↓
Prediction
 ↓
Loss
 ↓
Gradient
 ↓
Backpropagation
 ↓
Optimizer
 ↓
Weight Update

This helps build a stronger understanding of what Deep Learning frameworks are doing internally.

🔬 Upcoming Experiments

The next stage will focus on experimenting with the current ANN rather than immediately moving to another architecture.

Planned experiments:

 Compare different numbers of neurons
 Compare different ANN architectures
 Implement Mini-Batch training using DataLoader
 Compare SGD vs Adam
 Experiment with learning rates
 Compare activation functions
 Study overfitting and underfitting
 Introduce Dropout
 Experiment with batch size
 Implement validation data
 Implement early stopping
 Save and load trained models
 Perform single-customer inference
 Refactor the ANN into reusable training/evaluation functions
🗺️ Future Deep Learning Roadmap

After completing ANN experiments:

ANN
 │
 ├── Regularization
 ├── Dropout
 ├── Batch Normalization
 ├── Advanced Optimizers
 │
 ▼
CNN
 │
 ▼
Computer Vision
 │
 ▼
RNN
 │
 ▼
LSTM / GRU
 │
 ▼
Sequence Modeling
 │
 ▼
Attention
 │
 ▼
Transformers
 │
 ▼
Modern Deep Learning
🎯 Long-Term Goal

The long-term objective of this repository is to progress from fundamental neural networks to modern Deep Learning architectures.

Mathematics
     ↓
Neural Networks
     ↓
ANN
     ↓
CNN
     ↓
RNN / LSTM
     ↓
Attention
     ↓
Transformers
     ↓
Modern AI / GenAI

The ultimate goal is to understand not just how to use Deep Learning models, but why and how they work internally.

⭐ Progress
Deep Learning Fundamentals
 Perceptron
 Weights & Bias
 Weighted Sum
 Activation Functions
 Sigmoid
 Tanh
 ReLU
 Forward Propagation
 Loss Function
 Backpropagation
 Chain Rule
 Gradients
 Gradient Descent
 Learning Rate
 SGD
 Mini-Batch SGD concepts
 Optimizer concepts
 AdaGrad concepts
Artificial Neural Networks
 Multiple neurons
 Hidden layers
 ANN architecture
 PyTorch implementation
 Binary classification
 Training
 Loss visualization
 Model evaluation
 Classification report
 Confusion matrix
Current Project
 Customer Churn Dataset
 Data preprocessing
 Categorical encoding
 Train/Test split
 Feature scaling
 PyTorch tensors
 ANN model
 ReLU activation
 Sigmoid output
 BCELoss
 Adam optimizer
 Model training
 Accuracy evaluation
 Classification report
 Confusion matrix
Next
 ANN Architecture Experiments
 Mini-Batch DataLoader
 SGD vs Adam
 Learning Rate Experiments
 Activation Experiments
 Overfitting
 Dropout
 Batch Normalization
 Early Stopping
 Model Saving & Loading
 CNN
🚀 Status

Current Stage: Artificial Neural Network (ANN) using PyTorch

Learning Deep Learning by understanding the fundamentals, implementing them, and validating them through experiments.

provide a proper READMe.md as i need to push on gkithub so accordingly

Yes — for GitHub, the README should look like a real project repository README, not like personal study notes. It should clearly show what the repository is, what has been completed, the current ANN project, tech stack, structure, and roadmap.

Here is a cleaner, professional, GitHub-ready version based only on your current completed work.

# 🧠 Deep Learning From Scratch

> A hands-on journey to understand Deep Learning from first principles by studying the intuition, mathematics, implementation, and practical application of neural networks.

---

## 📌 About

This repository documents my journey of learning **Deep Learning from scratch**.

The goal is to understand what happens inside a neural network rather than treating Deep Learning frameworks as black boxes.

The learning approach is:

```text
Understand → Derive → Implement → Experiment → Use Frameworks

I started with the fundamentals of an artificial neuron and gradually progressed toward building an Artificial Neural Network (ANN) using PyTorch for a real-world Customer Churn Prediction problem.

The repository will continue to evolve toward more advanced Deep Learning architectures such as CNNs, RNNs, LSTMs, and Transformers.

🎯 Objectives

The main objectives of this repository are:

Understand the mathematical foundations of Deep Learning
Understand how artificial neurons work
Understand weights and biases
Understand activation functions
Understand forward propagation
Understand loss functions
Understand backpropagation
Understand the chain rule
Understand gradients
Understand gradient descent
Understand learning rates
Understand SGD and Mini-Batch SGD
Understand optimization algorithms
Build neural networks from first principles
Implement neural networks using PyTorch
Train models on real-world datasets
Evaluate and analyze model performance
Gradually progress toward modern Deep Learning architectures
📚 Topics Covered
Deep Learning Fundamentals
Artificial Neuron

Understanding the basic mathematical structure of a neuron:

z = w₁x₁ + w₂x₂ + ... + wₙxₙ + b

output = activation(z)
Weights & Bias

Understanding:

Weights
Bias
Weighted sum
Parameter learning
How parameters affect predictions
Activation Functions

Studied the purpose of activation functions and their role in introducing non-linearity.

Currently covered:

Sigmoid
Tanh
ReLU
Sigmoid
f(x) = 1 / (1 + e⁻ˣ)

Range:

0 → 1
Tanh
f(x) = tanh(x)

Range:

-1 → 1
ReLU
f(x) = max(0, x)
Forward Propagation

Understanding how information flows through a neural network:

Input
  ↓
Weighted Sum
  ↓
Activation
  ↓
Hidden Layer
  ↓
Output
Loss Function

Understanding how a neural network measures the difference between:

Prediction ↔ Actual Target

The objective of training is to minimize the loss.

Backpropagation

Understanding how gradients are calculated and propagated backward through the network.

Loss
 ↓
Gradients
 ↓
Parameters
 ↓
Parameter Updates
Chain Rule

Studied the mathematical foundation used by backpropagation to calculate gradients through multiple operations.

Gradient Descent

Understanding how parameters are updated to minimize the loss.

θnew = θold - learning_rate × gradient
Learning Rate

Understanding how the learning rate controls the size of parameter updates.

Large Learning Rate
        ↓
Possible Overshooting

Small Learning Rate
        ↓
Slow Convergence
SGD

Studied Stochastic Gradient Descent and how parameter updates can be performed using individual training samples.

Mini-Batch SGD

Studied how training can be performed using small batches of data instead of the entire dataset.

Dataset
   ↓
Mini-Batches
   ↓
Gradient Calculation
   ↓
Parameter Update
Optimization

Studied the role of optimizers in neural network training.

Currently covered:

Gradient Descent
SGD
Mini-Batch SGD
AdaGrad
Adam
🚀 Current Project
Customer Churn Prediction using PyTorch ANN

The current practical implementation is an Artificial Neural Network for Customer Churn Prediction.

The model predicts whether a customer is likely to leave a company.

Dataset
Churn_Modelling.csv
Target Variable
Exited
0 → Customer stays
1 → Customer exits
🔄 Machine Learning Pipeline

The complete workflow currently implemented is:

Raw Dataset
     │
     ▼
Data Cleaning
     │
     ▼
Feature / Target Separation
     │
     ▼
Categorical Encoding
     │
     ▼
Train / Test Split
     │
     ▼
Feature Scaling
     │
     ▼
NumPy → PyTorch Tensors
     │
     ▼
ANN
     │
     ▼
Training
     │
     ▼
Evaluation
🧹 Data Preprocessing

The following unnecessary columns are removed:

RowNumber
CustomerId
Surname

The target column is separated:

X = df.drop("Exited", axis=1)
y = df["Exited"]
🔤 Categorical Encoding

Categorical features are converted into numerical features using one-hot encoding.

X = pd.get_dummies(
    X,
    columns=["Geography", "Gender"],
    drop_first=True
)
✂️ Train/Test Split

The dataset is divided into:

80% → Training
20% → Testing

using:

X_train, X_test, y_train, y_test = train_test_split(
    X,
    y,
    test_size=0.2,
    random_state=42,
    stratify=y
)
📏 Feature Scaling

Features are standardized using StandardScaler.

scaler = StandardScaler()

X_train = scaler.fit_transform(X_train)
X_test = scaler.transform(X_test)

The scaler is fitted only on the training data to prevent data leakage.

🔢 PyTorch Tensors

The processed data is converted into PyTorch tensors:

X_train_tensor = torch.tensor(
    X_train,
    dtype=torch.float32
)

X_test_tensor = torch.tensor(
    X_test,
    dtype=torch.float32
)

y_train_tensor = torch.tensor(
    y_train,
    dtype=torch.float32
).reshape(-1, 1)

y_test_tensor = torch.tensor(
    y_test,
    dtype=torch.float32
).reshape(-1, 1)
🏗️ ANN Architecture

The current neural network architecture is:

Input Layer
     │
     │ 11 Features
     ▼
Linear Layer
11 → 16
     │
     ▼
ReLU
     │
     ▼
Linear Layer
16 → 8
     │
     ▼
ReLU
     │
     ▼
Linear Layer
8 → 1
     │
     ▼
Sigmoid
     │
     ▼
Churn Probability
Architecture Summary
11 → 16 → 8 → 1
💻 PyTorch Implementation
import torch
import torch.nn as nn


class ChurnANN(nn.Module):

    def __init__(self):
        super().__init__()

        self.layer1 = nn.Linear(11, 16)
        self.layer2 = nn.Linear(16, 8)
        self.output = nn.Linear(8, 1)

        self.relu = nn.ReLU()
        self.sigmoid = nn.Sigmoid()

    def forward(self, x):

        x = self.layer1(x)
        x = self.relu(x)

        x = self.layer2(x)
        x = self.relu(x)

        x = self.output(x)
        x = self.sigmoid(x)

        return x
📉 Loss Function

Binary Cross Entropy Loss is used for the current binary classification problem.

criterion = nn.BCELoss()

The model produces a probability between 0 and 1, which is compared against the actual binary target.

⚙️ Optimizer

The current implementation uses the Adam optimizer.

optimizer = torch.optim.Adam(
    model.parameters(),
    lr=0.001
)

Current learning rate:

0.001
🔥 Training

The current model is trained for:

100 epochs

The training process follows:

Input
  ↓
Forward Propagation
  ↓
Prediction
  ↓
Loss Calculation
  ↓
Backpropagation
  ↓
Gradient Calculation
  ↓
Adam Optimizer
  ↓
Weight Update
  ↓
Repeat
📊 Training Loss

Training loss is recorded after every epoch and visualized using Matplotlib.

loss_history = []

for epoch in range(epochs):

    predictions = model(X_train_tensor)

    loss = criterion(
        predictions,
        y_train_tensor
    )

    optimizer.zero_grad()

    loss.backward()

    optimizer.step()

    loss_history.append(loss.item())

The loss curve helps visualize whether the model is learning during training.

🧪 Model Evaluation

After training, the model is switched to evaluation mode:

model.eval()

Predictions are generated without calculating gradients:

with torch.no_grad():
    predictions = model(X_test_tensor)
🎯 Classification Threshold

The model outputs probabilities.

A threshold of 0.5 is used:

Prediction >= 0.5
        ↓
Customer Churn

Prediction < 0.5
        ↓
Customer Does Not Churn

Implementation:

predicted_classes = (
    predictions >= 0.5
).float()
📈 Evaluation Metrics

The model is evaluated using:

Accuracy

Measures the percentage of correctly classified samples.

Classification Report

The classification report provides:

Precision
Recall
F1-score
Support
classification_report(
    y_true,
    y_pred
)
Confusion Matrix

The confusion matrix helps understand the types of correct and incorrect predictions.

                 Predicted
                0       1

Actual  0      TN      FP

        1      FN      TP

Where:

TN → True Negative
FP → False Positive
FN → False Negative
TP → True Positive
🛠️ Tech Stack
Technology	Purpose
Python	Programming Language
NumPy	Numerical Computing
Pandas	Data Processing
Matplotlib	Visualization
Scikit-learn	Data Preprocessing & Evaluation
PyTorch	Deep Learning
Google Colab	Development Environment
Git & GitHub	Version Control
📂 Repository Structure
deep-learning-from-scratch/
│
├── README.md
│
├── ANN/
│   └── ANN_Customer_Churn_PyTorch.ipynb
│
└── datasets/
    └── Churn_Modelling.csv

The repository structure will be expanded as new Deep Learning architectures and experiments are added.

📈 Learning Progress
Deep Learning Fundamentals
 Artificial Neuron
 Weights
 Bias
 Weighted Sum
 Activation Functions
 Sigmoid
 Tanh
 ReLU
 Forward Propagation
 Loss Function
 Backpropagation
 Chain Rule
 Gradients
 Gradient Descent
 Learning Rate
 SGD
 Mini-Batch SGD
 Optimizer Concepts
 AdaGrad
 Adam
Artificial Neural Networks
 Multiple Neurons
 Hidden Layers
 ANN Architecture
 PyTorch ANN
 Binary Classification
 Model Training
 Loss Visualization
 Model Evaluation
 Classification Report
 Confusion Matrix
Customer Churn Project
 Dataset Loading
 Data Cleaning
 Feature Selection
 Categorical Encoding
 Train/Test Split
 Feature Scaling
 PyTorch Tensor Conversion
 ANN Architecture
 Model Training
 Adam Optimizer
 Accuracy Evaluation
 Classification Report
 Confusion Matrix
🔬 Upcoming Experiments

The next phase will focus on understanding how different choices affect ANN performance.

 Experiment with number of neurons
 Experiment with different ANN architectures
 Implement Mini-Batch training using DataLoader
 Compare SGD vs Adam
 Experiment with learning rates
 Compare activation functions
 Study overfitting and underfitting
 Implement Dropout
 Experiment with batch sizes
 Add validation data
 Implement Early Stopping
 Save and Load PyTorch models
 Perform single-sample inference
 Refactor training pipeline
 Move toward CNN
🗺️ Future Roadmap
Deep Learning Fundamentals
            │
            ▼
           ANN
            │
            ├── Optimization
            ├── Regularization
            ├── Dropout
            ├── Batch Normalization
            └── Training Experiments
            │
            ▼
           CNN
            │
            ▼
    Computer Vision
            │
            ▼
           RNN
            │
            ▼
        LSTM / GRU
            │
            ▼
    Sequence Modeling
            │
            ▼
        Attention
            │
            ▼
      Transformers
            │
            ▼
       Modern AI
🧠 Learning Philosophy

This repository follows a first-principles approach.

Instead of simply writing:

model.fit(...)

the objective is to understand what happens internally:

Input
  ↓
Weights & Bias
  ↓
Weighted Sum
  ↓
Activation Function
  ↓
Prediction
  ↓
Loss
  ↓
Gradient
  ↓
Backpropagation
  ↓
Optimizer
  ↓
Parameter Update

The purpose is to build a strong conceptual and mathematical foundation before moving toward advanced architectures.

🚀 Long-Term Goal

The long-term goal is to progress from the fundamentals of neural networks to modern Deep Learning and eventually Generative AI and Transformer-based systems.

Mathematics
    ↓
Neural Networks
    ↓
ANN
    ↓
CNN
    ↓
RNN / LSTM
    ↓
Attention
    ↓
Transformers
    ↓
Deep Learning
    ↓
Generative AI
⭐ Status

Current Stage: Artificial Neural Network (ANN) — PyTorch

Current Project: Customer Churn Prediction

Next Focus: ANN Experiments → Mini-Batch Training → Optimization → Regularization → CNN

👨‍💻 Author

Sarthak Rajvaidya

🚀 Learning Deep Learning one concept at a time — from mathematical foundations to modern AI systems.


### One important GitHub point

I would **not** put your actual `Churn_Modelling.csv` dataset into GitHub if you don't need to. Keep the notebook and README in the repo, and either:

```text
datasets/
└── README.md

with instructions for obtaining the dataset, or add the CSV to .gitignore if you're keeping it locally.

Also, for your next commit, a clean message would be:

git add README.md
git commit -m "docs: add project README"
git push

This README now represents your current stage honestly: fundamentals → optimization concepts → PyTorch ANN → customer churn project, while keeping the future CNN/advanced topics as a roadmap rather than claiming you've already completed them.

u provide me a readymade file i would copy that accordingly

Done. I created the ready-to-use README.md file for your GitHub repository.

📄 Download

Download README.md

Just replace your existing README.md with this file and push:

git add README.md
git commit -m "docs: update project README"
git push

It reflects your current completed work up to the PyTorch ANN Customer Churn project, while keeping the upcoming experiments and CNN/advanced Deep Learning as the roadmap. 

README.md
Document

Library
/
README.md
🧠 Deep Learning From Scratch

A hands-on journey to understand Deep Learning from first principles by studying the intuition, mathematics, implementation, and practical application of neural networks.

📌 About

This repository documents my journey of learning Deep Learning from scratch.

The goal is to understand what happens inside a neural network rather than treating Deep Learning frameworks as black boxes.

The learning approach is:

Understand → Derive → Implement → Experiment → Use Frameworks

I started with the fundamentals of an artificial neuron and gradually progressed toward building an Artificial Neural Network (ANN) using PyTorch for a real-world Customer Churn Prediction problem.

The repository will continue to evolve toward more advanced Deep Learning architectures such as CNNs, RNNs, LSTMs, and Transformers.

🎯 Objectives
Understand the mathematical foundations of Deep Learning
Understand how artificial neurons work
Understand weights and biases
Understand activation functions
Understand forward propagation
Understand loss functions
Understand backpropagation
Understand the chain rule
Understand gradients
Understand gradient descent
Understand learning rates
Understand SGD and Mini-Batch SGD
Understand optimization algorithms
Build neural networks from first principles
Implement neural networks using PyTorch
Train models on real-world datasets
Evaluate and analyze model performance
Progress toward modern Deep Learning architectures
📚 Topics Covered
Deep Learning Fundamentals
Artificial Neuron

The basic mathematical structure of a neuron:

z = w₁x₁ + w₂x₂ + ... + wₙxₙ + b

output = activation(z)
Weights & Bias

Understanding:

Weights
Bias
Weighted sum
Parameter learning
How parameters affect predictions
Activation Functions

Currently studied:

Sigmoid
Tanh
ReLU
Sigmoid
f(x) = 1 / (1 + e⁻ˣ)

Range: 0 → 1

Tanh
f(x) = tanh(x)

Range: -1 → 1

ReLU
f(x) = max(0, x)
Forward Propagation
Input
  ↓
Weighted Sum
  ↓
Activation
  ↓
Hidden Layer
  ↓
Output
Loss Function

Understanding how a neural network measures the difference between its prediction and the actual target.

Backpropagation

Understanding how gradients are calculated and propagated backward through the network.

Loss
 ↓
Gradients
 ↓
Parameters
 ↓
Parameter Updates
Chain Rule

Studied the mathematical foundation used by backpropagation to calculate gradients through multiple operations.

Gradient Descent
θnew = θold - learning_rate × gradient
Learning Rate

Understanding how the learning rate controls the size of parameter updates.

SGD

Studied Stochastic Gradient Descent and how parameter updates can be performed using individual training samples.

Mini-Batch SGD

Studied how training can be performed using small batches instead of the entire dataset.

Dataset
   ↓
Mini-Batches
   ↓
Gradient Calculation
   ↓
Parameter Update
Optimization

Studied the role of optimizers in neural network training.

Currently covered:

Gradient Descent
SGD
Mini-Batch SGD
AdaGrad
Adam
🚀 Current Project
Customer Churn Prediction using PyTorch ANN

The current practical implementation is an Artificial Neural Network for Customer Churn Prediction.

The model predicts whether a customer is likely to leave a company.

Dataset
Churn_Modelling.csv
Target Variable
Exited
0 → Customer stays
1 → Customer exits
🔄 Machine Learning Pipeline
Raw Dataset
     │
     ▼
Data Cleaning
     │
     ▼
Feature / Target Separation
     │
     ▼
Categorical Encoding
     │
     ▼
Train / Test Split
     │
     ▼
Feature Scaling
     │
     ▼
NumPy → PyTorch Tensors
     │
     ▼
ANN
     │
     ▼
Training
     │
     ▼
Evaluation
🧹 Data Preprocessing

The following unnecessary columns are removed:

RowNumber
CustomerId
Surname

The target column is separated:

X = df.drop("Exited", axis=1)
y = df["Exited"]
Categorical Encoding

Categorical features are converted into numerical features using one-hot encoding.

X = pd.get_dummies(
    X,
    columns=["Geography", "Gender"],
    drop_first=True
)
Train/Test Split

The dataset is divided into:

80% → Training
20% → Testing

using:

X_train, X_test, y_train, y_test = train_test_split(
    X,
    y,
    test_size=0.2,
    random_state=42,
    stratify=y
)
Feature Scaling

Features are standardized using StandardScaler.

scaler = StandardScaler()

X_train = scaler.fit_transform(X_train)
X_test = scaler.transform(X_test)

The scaler is fitted only on the training data to prevent data leakage.

PyTorch Tensors

The processed data is converted into PyTorch tensors.

X_train_tensor = torch.tensor(
    X_train,
    dtype=torch.float32
)

X_test_tensor = torch.tensor(
    X_test,
    dtype=torch.float32
)

y_train_tensor = torch.tensor(
    y_train,
    dtype=torch.float32
).reshape(-1, 1)

y_test_tensor = torch.tensor(
    y_test,
    dtype=torch.float32
).reshape(-1, 1)
🏗️ ANN Architecture

The current neural network architecture is:

Input Layer
     │
     │ 11 Features
     ▼
Linear Layer
11 → 16
     │
     ▼
ReLU
     │
     ▼
Linear Layer
16 → 8
     │
     ▼
ReLU
     │
     ▼
Linear Layer
8 → 1
     │
     ▼
Sigmoid
     │
     ▼
Churn Probability
Architecture Summary
11 → 16 → 8 → 1
💻 PyTorch Implementation
import torch
import torch.nn as nn


class ChurnANN(nn.Module):

    def __init__(self):
        super().__init__()

        self.layer1 = nn.Linear(11, 16)
        self.layer2 = nn.Linear(16, 8)
        self.output = nn.Linear(8, 1)

        self.relu = nn.ReLU()
        self.sigmoid = nn.Sigmoid()

    def forward(self, x):

        x = self.layer1(x)
        x = self.relu(x)

        x = self.layer2(x)
        x = self.relu(x)

        x = self.output(x)
        x = self.sigmoid(x)

        return x
📉 Loss Function

Binary Cross Entropy Loss is used for the current binary classification problem.

criterion = nn.BCELoss()
⚙️ Optimizer

The current implementation uses the Adam optimizer.

optimizer = torch.optim.Adam(
    model.parameters(),
    lr=0.001
)

Current learning rate:

0.001
🔥 Training

The current model is trained for:

100 epochs

The training process follows:

Input
  ↓
Forward Propagation
  ↓
Prediction
  ↓
Loss Calculation
  ↓
Backpropagation
  ↓
Gradient Calculation
  ↓
Adam Optimizer
  ↓
Weight Update
  ↓
Repeat

Training loss is recorded after every epoch and visualized using Matplotlib.

🧪 Model Evaluation

After training, the model is switched to evaluation mode:

model.eval()

Predictions are generated without calculating gradients:

with torch.no_grad():
    predictions = model(X_test_tensor)
Classification Threshold

A threshold of 0.5 is used:

Prediction >= 0.5
        ↓
Customer Churn

Prediction < 0.5
        ↓
Customer Does Not Churn
📈 Evaluation Metrics

The model is evaluated using:

Accuracy
Precision
Recall
F1-score
Confusion Matrix
Confusion Matrix
                 Predicted
                0       1

Actual  0      TN      FP

        1      FN      TP

Where:

TN → True Negative
FP → False Positive
FN → False Negative
TP → True Positive
🛠️ Tech Stack
Technology	Purpose
Python	Programming Language
NumPy	Numerical Computing
Pandas	Data Processing
Matplotlib	Visualization
Scikit-learn	Preprocessing & Evaluation
PyTorch	Deep Learning
Google Colab	Development Environment
Git & GitHub	Version Control
📂 Repository Structure
deep-learning-from-scratch/
│
├── README.md
│
├── ANN/
│   └── ANN_Customer_Churn_PyTorch.ipynb
│
└── datasets/
    └── Churn_Modelling.csv

The repository structure will expand as new Deep Learning architectures and experiments are added.

📈 Learning Progress
Deep Learning Fundamentals

Artificial Neuron

Weights & Bias

Weighted Sum

Activation Functions

Sigmoid

Tanh

ReLU

Forward Propagation

Loss Function

Backpropagation

Chain Rule

Gradients

Gradient Descent

Learning Rate

SGD

Mini-Batch SGD

Optimizer Concepts

AdaGrad

Adam

Artificial Neural Networks

Multiple Neurons

Hidden Layers

ANN Architecture

PyTorch ANN

Binary Classification

Model Training

Loss Visualization

Model Evaluation

Classification Report

Confusion Matrix

Customer Churn Project

Dataset Loading

Data Cleaning

Feature Selection

Categorical Encoding

Train/Test Split

Feature Scaling

PyTorch Tensor Conversion

ANN Architecture

Model Training

Adam Optimizer

Accuracy Evaluation

Classification Report

Confusion Matrix

🔬 Upcoming Experiments

The next phase will focus on understanding how different choices affect ANN performance.

Experiment with number of neurons

Experiment with different ANN architectures

Implement Mini-Batch training using DataLoader

Compare SGD vs Adam

Experiment with learning rates

Compare activation functions

Study overfitting and underfitting

Implement Dropout

Experiment with batch sizes

Add validation data

Implement Early Stopping

Save and Load PyTorch models

Perform single-sample inference

Refactor training pipeline

Move toward CNN

🗺️ Future Roadmap
Deep Learning Fundamentals
            │
            ▼
           ANN
            │
            ├── Optimization
            ├── Regularization
            ├── Dropout
            ├── Batch Normalization
            └── Training Experiments
            │
            ▼
           CNN
            │
            ▼
    Computer Vision
            │
            ▼
           RNN
            │
            ▼
        LSTM / GRU
            │
            ▼
    Sequence Modeling
            │
            ▼
        Attention
            │
            ▼
      Transformers
            │
            ▼
       Modern AI
🧠 Learning Philosophy

This repository follows a first-principles approach.

Instead of simply using high-level APIs, the objective is to understand what happens internally:

Input
  ↓
Weights & Bias
  ↓
Weighted Sum
  ↓
Activation Function
  ↓
Prediction
  ↓
Loss
  ↓
Gradient
  ↓
Backpropagation
  ↓
Optimizer
  ↓
Parameter Update

The purpose is to build a strong conceptual and mathematical foundation before moving toward advanced architectures.

🚀 Long-Term Goal

The long-term goal is to progress from the fundamentals of neural networks to modern Deep Learning and eventually Generative AI and Transformer-based systems.

Mathematics
    ↓
Neural Networks
    ↓
ANN
    ↓
CNN
    ↓
RNN / LSTM
    ↓
Attention
    ↓
Transformers
    ↓
Deep Learning
    ↓
Generative AI
⭐ Current Status

Current Stage: Artificial Neural Network (ANN) — PyTorch

Current Project: Customer Churn Prediction

Next Focus: ANN Experiments → Mini-Batch Training → Optimization → Regularization → CNN

👨‍💻 Author

Sarthak Rajvaidya

🚀 Learning Deep Learning one concept at a time — from mathematical foundations to modern AI systems.
