# 🏡 House Price Prediction using Linear Regression

## 📌 Overview
This project applies **Linear Regression** to predict house prices based on key features such as lot size, overall quality, number of rooms, and more.  
It uses the **Kaggle House Prices dataset** (train and test CSV files) and generates predictions saved in a submission file.

---

## 📂 Project Structure
```
├── house_prices_train.csv   # Training dataset
├── house_prices_test.csv    # Test dataset
├── house_price_results.csv  # Output predictions (submission file)
├── house_price_model.py     # Main Python script
└── README.md                # Project documentation
```

---

## ⚙️ Features Used
The model uses the following predictors:

- `MSSubClass`  
- `LotArea`  
- `OverallQual`  
- `OverallCond`  
---

## 🚀 Workflow
1. **Data Loading**  
   - Training and test datasets are loaded using `pandas`.

2. **Feature Selection & Preprocessing**  
   - Selected features are extracted.  
   - Missing values are handled using **mean imputation** (`SimpleImputer`).

3. **Model Training**  
   - A **Linear Regression** model is trained on the imputed training data.

4. **Evaluation**  
   - Model performance is measured using **Mean Squared Error (MSE)** and **R² Score**.

5. **Prediction & Submission**  
   - Predictions are generated for the test dataset.  
   - Results are saved to `house_price_results.csv`.

6. **Visualization**  
   - A scatter plot compares **actual vs predicted prices** for the training set.

---

## 📊 Visualization
The script generates a plot showing how well the model fits the training data:

- **Blue scatter points** → Predicted vs Actual values  
- **Dashed red line** → Perfect prediction reference  

This helps visually assess model accuracy.

---

## 🛠️ Requirements
Install the following dependencies before running the script:

```bash
pip install pandas numpy matplotlib scikit-learn
```

---

## ▶️ Usage
Run the script with:

```bash
python house_price_model.py
```

- Ensure `house_prices_train.csv` and `house_prices_test.csv` are in the same directory.  
- The output file `house_price_results.csv` will be generated automatically.

---

## 📈 Example Output
```
Training Evaluation:
Mean Squared Error: 1.23e+09
R² Score: 0.82

File saved as: house_price_results.csv
```

---

