# Deep Learning: From Basics to Projects

[![Python](https://img.shields.io/badge/Python-3.10%E2%80%933.12-blue.svg)](https://www.python.org/)
[![TensorFlow](https://img.shields.io/badge/TensorFlow-Keras-orange.svg)](https://www.tensorflow.org/)
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/YOUR-USERNAME/Deep-Learning/blob/main/notebooks/01_first_neural_network.ipynb)

A beginner-friendly, hands-on repository for learning Deep Learning with Python, NumPy, TensorFlow, and Keras. Read the notes, run the code, change one thing at a time, and build your own projects.

## Table of Contents
- [What you'll learn](#what-youll-learn)
- [Prerequisites](#prerequisites)
- [Repository structure](#repository-structure)
- [Setup](#setup)
- [Run the example](#run-the-example)
- [Learning order](#learning-order)
- [Experiment log](#experiment-log)
- [Core concepts checklist](#core-concepts-checklist)
- [Good habits](#good-habits)
- [Next steps and resources](#next-steps-and-resources)
- [Contributing](#contributing)
- [License](#license)

## What you'll learn
- Deep Learning fundamentals and neural-network terminology
- Tensors, layers, weights, biases, activation functions, loss, and optimizers
- Forward propagation, backpropagation, and gradient descent
- Training, validation, testing, overfitting, regularization, and evaluation
- Practical workflows with TensorFlow/Keras
- Starter projects for image classification and tabular data

## Prerequisites
- Basic Python (functions, loops, lists, and dictionaries)
- A little NumPy (arrays, shapes, indexing)
- High-school-level math: vectors, matrices, and the idea of a derivative

No prior machine learning experience is needed.

## Repository structure
```text
Deep-Learning/
├── README.md
├── LICENSE
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

### 1. Clone the repository
```bash
git clone https://github.com/YOUR-USERNAME/Deep-Learning.git
cd Deep-Learning
```

### 2. Create and activate a virtual environment
Use a Python version supported by TensorFlow (3.10–3.12 at the time of writing; check the [TensorFlow install guide](https://www.tensorflow.org/install/pip) for the current list).

**Windows (PowerShell or Command Prompt):**
```bash
py -m venv .venv
.venv\Scripts\activate
```

**macOS / Linux:**
```bash
python3 -m venv .venv
source .venv/bin/activate
```

### 3. Install packages
```bash
python -m pip install --upgrade pip
pip install -r requirements.txt
```

> **Trouble installing TensorFlow?** Check the TensorFlow installation guide for your operating system and Python version, or skip local setup and run the notebook in Google Colab using the badge at the top.

## Run the example
```bash
python src/mnist_classifier.py
```
The script downloads the MNIST dataset on first run, trains a small neural network, evaluates it on the test set, and saves the model as `mnist_model.keras`.

**What to expect:** training takes a minute or two on a typical laptop CPU, and test accuracy should land roughly in the high 90s (about 97–98%). Exact numbers vary between runs.

> `mnist_model.keras` and downloaded datasets are generated files. They are listed in `.gitignore` and should not be committed.

## Learning order
1. Read the notes in `NOTES/`.
2. Run the notebook cell by cell and explain each line in your own words.
3. Run the MNIST example.
4. Change one thing at a time: number of epochs, hidden units, batch size, or optimizer.
5. Record test accuracy and observations in your own experiment log.
6. Build one project independently (see `projects/PROJECT_IDEAS.md`) and document its limitations.

See [`ROADMAP.md`](ROADMAP.md) for a longer-term plan.

## Experiment log
Keep a simple table like this (in a notebook, a markdown file, or a spreadsheet) so you can see what actually helped:

| # | Change | Epochs | Hidden units | Batch size | Optimizer | Val accuracy | Test accuracy | Notes |
|---|--------|--------|--------------|------------|-----------|--------------|---------------|-------|
| 1 | Baseline | | | | | | | |
| 2 | | | | | | | | |

## Core concepts checklist
Fork the repo or copy this list into your own notes to tick items off as you learn them.

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

## Next steps and resources
- [TensorFlow tutorials](https://www.tensorflow.org/tutorials)
- [Keras documentation](https://keras.io/guides/)
- [Deep Learning Specialization](https://www.deeplearning.ai/) and [fast.ai](https://course.fast.ai/) courses
- *Deep Learning with Python* by François Chollet

## Contributing
Found a typo, an unclear explanation, or a broken step? Please open an issue or a pull request. Suggested commit message style:

- `docs: add deep learning roadmap`
- `feat: add first keras neural network`
- `docs: explain activation functions`
- `feat: add mnist classifier`
- `docs: record model evaluation results`

## License
This project is licensed under the [MIT License](LICENSE). Add a `LICENSE` file containing the MIT text with your name and the year.
