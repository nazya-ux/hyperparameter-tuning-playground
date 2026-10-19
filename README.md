# Hyperparameter Tuning Playground 🔬

A beginner-friendly machine learning project comparing **Grid Search and Random Search** for hyperparameter optimization using a Random Forest classifier.

## 🎯 Objective

Explore how different hyperparameter search strategies affect model performance and computational cost.

## 🛠️ Tech Stack

- Python
- Jupyter Notebook
- NumPy and Pandas
- Matplotlib
- Scikit-learn

## 📊 Dataset

The project uses the Breast Cancer Wisconsin dataset available through Scikit-learn.

- 569 samples
- 30 numerical features
- Binary classification: malignant or benign
- 80% training data and 20% test data

## 🧪 Methodology

1. Load and explore the dataset.
2. Split the data into training and test sets.
3. Train a baseline Random Forest classifier.
4. Use Grid Search to evaluate 18 hyperparameter combinations with 5-fold cross-validation.
5. Use Random Search to evaluate 10 combinations with 5-fold cross-validation.
6. Compare cross-validation accuracy, test accuracy, F1 score, and search time.
7. Visualize performance using bar charts and confusion matrices.

## 📈 Results

| Metric | Baseline | Grid Search | Random Search |
|---|---:|---:|---:|
| Test accuracy | 95.61% | 95.61% | 95.61% |
| Test F1 score | 96.55% | 96.55% | 96.55% |
| Search time | No search | 11.23 s | 1.99 s |

Both search methods achieved 96.04% best cross-validation accuracy.

Random Search was approximately **5.64 times faster** in this experiment while achieving the same reported test metrics.

## 💡 Key Learnings

- Hyperparameters control how a machine learning algorithm learns.
- Cross-validation provides a more robust way to compare model configurations.
- Grid Search exhaustively evaluates the specified candidate combinations.
- Random Search explores a subset of candidate combinations.
- More tuning does not necessarily improve test performance when the baseline is already strong.
- Search time and predictive performance are separate considerations.

## ⚠️ Limitations

- Results come from one dataset and one train-test split.
- Runtime depends on hardware and system load.
- The selected hyperparameter ranges affect which configurations can be discovered.
- The experiment does not establish that one search method is always superior.

## 🚀 How to Run

1. Clone this repository.
2. Install the dependencies listed in `requirements.txt`.
3. Launch JupyterLab.
4. Open `notebooks/hyperparameter_tuning.ipynb`.
5. Run the notebook cells in order.

## 📁 Project Structure

```text
hyperparameter-tuning-playground/
├── notebooks/
│   └── hyperparameter_tuning.ipynb
├── results/
├── requirements.txt
└── README.md
```

## Disclaimer

This is an educational machine learning project, not a clinically validated diagnostic tool.