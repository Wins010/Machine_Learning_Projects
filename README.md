# 🚗 Simple Linear Regression — Auto MPG Dataset

This project demonstrates a **manual implementation of simple linear regression** using the classic [Auto MPG dataset](https://www.kaggle.com/datasets/uciml/autompg-dataset).  
The goal is to **predict a car’s fuel efficiency (MPG)** from its **horsepower**.

---

## 📂 Project Structure

```text
slr-auto-mpg/                      # Simple Linear Regression
│
├── README.md                      # Project overview, dataset info, instructions
├── requirements.txt               # Dependencies (pandas, numpy, matplotlib, sklearn, jupyter)
│
├── data/
│   ├── processed/
│   │   └── auto-mpg-clean.csv     # Cleaned dataset (after handling missing values, preprocessing)
│   └── raw/
│       └── auto-mpg.csv           # Original dataset (untouched)
│
└── notebooks/
    ├── 01_EDA.ipynb               # Exploratory Data Analysis (EDA) - distributions, correlations, plots
    └── 02_model_training.ipynb    # Model training & evaluation - fit SLR, plot regression line, compute metrics
```

---

## ⚙️ Workflow

1. **Exploratory Data Analysis (01_EDA.ipynb)**
   - Inspected dataset
   - Cleaned `horsepower` column (removed missing values, converted to numeric)
   - Explored distributions and scatterplots

2. **Model Training (02_model_training.ipynb)**
   - Implemented linear regression manually using NumPy:
   - Computed predictions
   - Evaluated model with R², MSE, MAE
   - Visualized regression line and residuals
   - Cross-checked with `scikit-learn` implementation

---

## 📊 Results

- **Slope (m):** ~ -0.158  
- **Intercept (b):** ~ 39.94  
- **R²:** ~0.61  
- **MSE:** ~23.9  
- **MAE:** ~3.8 MPG  

➡️ Interpretation:  
- Cars with higher horsepower tend to have lower MPG (negative slope).  
- Horsepower alone explains ~61% of the variance in MPG.  
- On average, predictions are within ~3.8 MPG of actual values.

---

## ▶️ How to Run

1. Clone this repo:
   ```bash
   git clone https://github.com/Wins010/Machine_Learning_Projects
   cd Supervised-Learning/Linear-Regression/Simple-Linear-Regression
   ```
2. Install dependencies:
   ```bash
    pip install -r requirements.txt
