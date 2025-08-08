# 🚗 CO₂ Emissions Regression Modeling – IBM Machine Learning Course 2 Final Project

## 📜 Project Overview
This project is part of the **IBM Machine Learning Professional Certificate – Course 2: Regression** final submission requirement.  
It involves performing **Exploratory Data Analysis (EDA)**, **feature preprocessing**, **regression modeling**, and **model comparison** to predict **vehicle CO₂ emissions** based on their specifications.

The analysis uses the **CO₂ Emissions Dataset (Canada)**, which contains detailed fuel consumption and engine specifications for thousands of vehicles.  
The main objective is to **determine which vehicle features most influence CO₂ output** and to **build accurate predictive models** for emissions estimation.

---

## 📚 IBM Course 2 Project Requirements
According to the **IBM ML Course 2 – Regression** final project guidelines, the submission must include:

1. **Data Understanding**
   - Describe dataset source, size, and variables.
   - Provide basic statistics and detect missing values.
   - Identify categorical and numerical variables.

2. **Exploratory Data Analysis (EDA)**
   - Visualize distributions and relationships.
   - Check correlations and detect outliers.
   - Summarize initial insights.

3. **Feature Engineering & Preprocessing**
   - Handle missing data (if any).
   - Encode categorical variables.
   - Scale/normalize numerical features.
   - Split into training/testing sets.

4. **Model Development**
   - Train at least **three regression models** (Linear, Ridge, Lasso).
   - Use pipelines for preprocessing + modeling.
   - Tune hyperparameters (if applicable).

5. **Model Evaluation**
   - Compare models using **R²**, **RMSE**, and **MAE**.
   - Present results in a clear comparison table and/or visualization.

6. **Key Insights**
   - Identify which features influence the target variable most.
   - Provide interpretation of model results.

7. **Limitations & Next Steps**
   - Discuss dataset and modeling limitations.
   - Suggest improvements and future directions.

---

## 📂 Dataset Information

**Dataset Name:** CO₂ Emissions – Canada (Government of Canada Open Data)  
**Rows:** 7,385  
**Columns:** 12  

**Key Variables**
- `Make` – Manufacturer
- `Model` – Vehicle model
- `Vehicle Class` – Vehicle type (SUV, Sedan, etc.)
- `Engine Size (L)` – Engine displacement in litres
- `Cylinders` – Number of engine cylinders
- `Transmission` – Gearbox type
- `Fuel Type` – Type of fuel used
- `Fuel Consumption City/Hwy/Comb` – Fuel efficiency metrics
- `CO2 Emissions (g/km)` – **Target variable**

---

## 🔍 Data Summary & Observations
- **No missing values** detected.
- Strong positive correlation between:
  - `Engine Size (L)` & CO₂ Emissions
  - `Fuel Consumption Comb (L/100 km)` & CO₂ Emissions
- Distribution of CO₂ emissions is **right-skewed**.
- Diverse vehicle classes ensure variability in target.

---

## 🛠️ Preprocessing Steps
- **Encoding**: One-Hot Encoding for categorical features.
- **Scaling**: StandardScaler for numerical features.
- **Splitting**: 80% training / 20% testing.

---

## 📈 Models Trained
1. **Linear Regression (OLS)** – Baseline model.
2. **Ridge Regression** – L2 regularization to handle multicollinearity.
3. **Lasso Regression** – L1 regularization with feature selection.

---

## 📊 Model Performance

| Model              | R² Score | RMSE  | MAE  |
|--------------------|---------:|------:|-----:|
| Linear Regression  | 0.9897   | 5.96  | 3.07 |
| Ridge Regression   | 0.9897   | 5.95  | 3.07 |
| Lasso Regression   | 0.9897   | 5.95  | 3.07 |

**Interpretation:**
- All models performed nearly identically.
- Low RMSE (~5.95) indicates high predictive accuracy.
- Regularization did not significantly improve performance but may improve generalization on unseen data.

---

## 💡 Key Insights
- **Fuel Consumption Comb (L/100 km)** is the strongest predictor of CO₂ emissions.
- Larger engines and more cylinders generally result in higher emissions.
- Well-structured linear models can achieve excellent performance for this dataset.

---

## ⚠️ Limitations
- **Feature depth**: Lacks vehicle weight, aerodynamics, and efficiency metrics.
- **No time dimension**: Can’t analyze trends over years.
- **Assumption of linearity**: May not capture complex interactions.

---

## 🚀 Future Work
- Test **tree-based models** (Random Forest, XGBoost).
- Apply **SHAP** for better feature interpretability.
- Build a **web app** for interactive emissions prediction.
- Incorporate **policy simulations** for emission reduction strategies.

---

## 📦 Project Structure
```

CO2\_Emissions\_Project/
│── data/                           # Dataset files
│── results/                        # Output results
│── images/                         # Plots and charts
│── models/                         # Saved models
│── notebooks/                      # Jupyter/Colab notebooks
│── README.md                       # Project documentation

```

---

## 🖼️ Sample Output Visualization
**Model Performance Comparison**
![Model Comparison](/images/download - 2025-08-07T230239.746.png)

---

## 🏫 Submission Notes (IBM Course 2)
- ✅ All 7 required sections completed.
- ✅ Three regression models implemented.
- ✅ Preprocessing included categorical encoding + scaling.
- ✅ Results presented with visualizations.
- ✅ Insights and limitations discussed.
- ✅ Suitable for both **academic submission** and **portfolio showcase**.

---

## 👨‍💻 Author
**Tamaghna Nag**  
London, UK | Kolkata, India  
[Portfolio](https://tamaghnatech.in) | [GitHub](https://github.com/Tamaghnatech)

