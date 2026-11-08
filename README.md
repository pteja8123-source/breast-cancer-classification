# SkillAudit.ai | Week 1: First ML Model with scikit-learn

A beginner-friendly binary classification project using the **Wisconsin Breast Cancer dataset** built into scikit-learn. This assignment compares Logistic Regression and Random Forest using a reproducible, stratified train/test split.

> **Educational use only:** This project is a machine-learning learning exercise. It is not a medical diagnostic system and must not be used to make healthcare decisions.

## Project objectives

- Load and explore a real-world classification dataset.
- Split data into training and testing subsets using stratification.
- Train Logistic Regression with a `StandardScaler` pipeline.
- Train a Random Forest classifier.
- Compare accuracy, precision, recall, and F1-score.
- Visualize accuracy and confusion matrices.
- Explore Random Forest feature importances.

## Dataset

The dataset is provided by `sklearn.datasets.load_breast_cancer()`.

- **Samples:** 569
- **Features:** 30 numeric features
- **Classes:** Malignant and benign
- **Target encoding:** `0 = malignant`, `1 = benign`

## Models

1. **Logistic Regression** using a pipeline with `StandardScaler`.
2. **Random Forest Classifier** using 300 trees.

Both experiments use `random_state=42`. The data is split into 80% training and 20% testing with stratification.

## Evaluation

The notebook reports:

- Accuracy
- Precision
- Recall
- F1-score
- Classification reports
- Confusion matrices

Precision, recall, and F1-score in the comparison table treat **malignant (class 0)** as the positive class. This makes malignant-class recall easy to interpret for this educational exercise. Results are calculated on the held-out test split and should not be interpreted as clinical performance.

## Repository contents

```text
skill-audit-week1-ml/
├── skill-audit-week1-ml.ipynb
└── README.md
```

## Run the notebook

### Google Colab

1. Download `skill-audit-week1-ml.ipynb` from this repository.
2. Open [Google Colab](https://colab.research.google.com/).
3. Select **File → Upload notebook**.
4. Upload the notebook.
5. Select **Runtime → Run all**.

### Local Jupyter environment

Install the dependencies:

```bash
pip install numpy pandas matplotlib seaborn scikit-learn jupyter
```

Launch Jupyter:

```bash
jupyter notebook
```

Open `skill-audit-week1-ml.ipynb` and run all cells.

## Results

Run the notebook to generate the actual metrics and plots. The notebook compares both models using the same test set. No performance numbers are hard-coded in this README.

## Limitations

- Evaluation uses one train/test split; results may vary with another split.
- The dataset is relatively small and may not represent real-world populations.
- No external validation, clinical review, or prospective testing is performed.
- Feature importance is a model-specific measure, not evidence of causation or medical significance.
- These models are not suitable for diagnosis, screening, treatment, or other medical decisions.

## Acknowledgement

Prepared as part of the **SkillAudit.ai Internship, Week 1 ML Assignment**.

## License

This repository contains an educational notebook. Check the dataset's original terms and any applicable scikit-learn licensing information before redistributing dataset-derived material.
