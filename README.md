# Deep-Learning
Learning Deep Learning with Python, TensorFlow, and Keras through notes, neural networks, hands-on notebooks, and practical projects.
# Deep Learning: From Basics to Projects

A beginner-friendly, hands-on repository for learning Deep Learning with Python, NumPy, TensorFlow, and Keras.

## What you'll learn
- Deep Learning fundamentals and neural-network terminology
- Tensors, layers, weights, biases, activation functions, loss, and optimizers
- Forward propagation, backpropagation, and gradient descent
- Training, validation, testing, overfitting, regularization, and evaluation
- Practical workflows with TensorFlow/Keras
- Starter projects for image classification and tabular data

## Repository structure
```text
Deep-Learning/
├── README.md
├── requirements.txt
├── .gitignore
├── ROADMAP.md
├── NOTES/
│   ├── 01_deep_learning_basics.md
│   ├── 02_neural_networks.md
│   ├── 03_training_and_evaluation.md
│   └── 04_cnn_basics.md
├── notebooks/
│   └── 01_first_neural_network.ipynb
├── src/
│   └── mnist_classifier.py
└── projects/
    └── PROJECT_IDEAS.md
```

## Setup

### 1. Clone your repository
After creating this repository on GitHub:
```bash
git clone https://github.com/YOUR-USERNAME/Deep-Learning.git
cd Deep-Learning
```

### 2. Create and activate a virtual environment
Windows:
```bash
py -3.11 -m venv .venv
.venv\\Scripts\\activate
```
macOS/Linux:
```bash
python3 -m venv .venv
source .venv/bin/activate
```

### 3. Install packages
```bash
python -m pip install --upgrade pip
pip install -r requirements.txt
```

> If TensorFlow installation fails, check the current TensorFlow installation guide for your operating system and Python version. You can also run the notebook in Google Colab.

## Run the example
```bash
python src/mnist_classifier.py
```
The script downloads the MNIST dataset on first run, trains a small neural network, evaluates it on the test set, and saves the model as `mnist_model.keras`.

## Learning order
1. Read the notes in `NOTES/`.
2. Run the notebook cell by cell and explain each line in your own words.
3. Run the MNIST example.
4. Change one thing at a time: number of epochs, hidden units, batch size, or optimizer.
5. Record test accuracy and observations in your own experiment log.
6. Build one project independently and document limitations.

## Core concepts checklist
- [ ] Tensors and tensor shapes
- [ ] Neurons, layers, weights, and biases
- [ ] Activation functions: ReLU, sigmoid, tanh, softmax
- [ ] Forward propagation and backpropagation
- [ ] Loss functions and optimizers
- [ ] Epoch, batch size, and learning rate
- [ ] Train/validation/test split
- [ ] Overfitting, underfitting, dropout, early stopping
- [ ] Classification metrics and confusion matrix
- [ ] Save and load a trained model

## Good habits
- Keep the test set separate until final evaluation.
- Fit preprocessing only on training data to avoid data leakage.
- Set random seeds when you want more repeatable experiments.
- Compare against a simple baseline.
- Do not report accuracy alone when classes are imbalanced.
- Document dataset source, preprocessing, metrics, and limitations.
- Never upload API keys, passwords, private data, or large datasets unnecessarily.

## Suggested commit messages
- `docs: add deep learning roadmap`
- `feat: add first keras neural network`
- `docs: explain activation functions`
- `feat: add mnist classifier`
- `docs: record model evaluation results`

## License
This repository is intended for learning. Add a license such as MIT if you want others to reuse your work; review the license terms before publishing.
