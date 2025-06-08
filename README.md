# ML Titanic Kaggle Contest 🚢

This project is part of the [Kaggle Titanic: Machine Learning from Disaster](https://www.kaggle.com/competitions/titanic/overview) competition. The goal is to use machine learning techniques to predict whether a passenger survived the sinking of the RMS Titanic based on available data.

With this model, we aim to explore feature engineering, classification algorithms, and performance evaluation in a real-world dataset.

---

## 📊 Dataset Overview

The dataset includes two files:

- `train.csv`: Contains labeled data with survival outcomes.
- `test.csv`: Data without survival labels used for final predictions.

### Features Description

| Feature       | Description |
|---------------|-------------|
| **survival**  | Whether the passenger survived (0 = No, 1 = Yes) |
| **pclass**    | Socio-economic status (SES): <br> - 1st = Upper <br> - 2nd = Middle <br> - 3rd = Lower |
| **age**       | Age in years |
| **sex**       | Sex of the passenger |
| **sibsp**     | Number of siblings or spouses aboard: <br> - Sibling = brother, sister, stepbrother, stepsister <br> - Spouse = husband, wife |
| **parch**     | Number of parents or children aboard: <br> - Parent = mother, father <br> - Child = daughter, son, stepdaughter, stepson <br> - Some children traveled only with a nanny (parch=0) |
| **ticket**    | Ticket number |
| **fare**      | Passenger fare |
| **cabin**     | Cabin number |
| **embarked**  | Port of embarkation: <br> - C = Cherbourg <br> - Q = Queenstown <br> - S = Southampton |

---

## Project Goals

- Perform exploratory data analysis (EDA) to understand patterns and correlations.
- Clean and preprocess data (handle missing values, encode categorical features).
- Build and evaluate classification model (e.g., Random Forest) with metrics.
- Generate predictions for the test set and submit to Kaggle for scoring.

---

## 🛠️ Technologies Used

- Python 3.11
- Pandas
- NumPy
- Scikit-learn
    - Joblib # for model reusage
- Scipy
- Matplotlib / Seaborn (for visualization)
- Jupyter Notebook

---

## 📁 File Structure

```
.
├── data/
│   ├── train.csv        # Training data
│   └── test.csv         # Test data
├── job lib models/      # Used models
│   └── Age_RF_predictor.joblib # For age NA filing
├── notebooks/
|   ├── Age regressor notebook/ 
│   │    └── Age_regressor.ipynb # Notebook for na filling
│   └── ML titanic prediction/
│       └── titanic_model.ipynb  # Main notebook for EDA and modeling
├── submission.csv       # Final prediction file for Kaggle submission
└── README.md            # This file
```

---

## Results

This version achieved a score of **0.77751** on the Kaggle leaderboard, placing within a competitive range among thousands of submissions.

---

## ▶️ How to Run

1. Clone the repository:

```bash
git clone https://github.com/PigStep/ML-Titanic-Kaggle-contest-0.77751.git
cd ML-Titanic-Kaggle-contest-0.77751
```

2. Install dependencies:

```bash
pip install pandas numpy scikit-learn matplotlib seaborn jupyter
```

3. Launch Jupyter Notebook:

```bash
jupyter notebook
```

4. Open `notebooks/titanic_model.ipynb` and run the cells to reproduce the analysis and generate predictions.

5. The final submission file (`submission.csv`) will be generated in the root directory.

---

## Feedback & Contributions

Contributions are welcome! If you have any suggestions or improvements, feel free to open an issue or submit a pull request.

---
