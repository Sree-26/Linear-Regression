# Linear Regression on Diabetes Dataset 🧠📊

This project demonstrates a complete workflow of applying Linear Regression to predict disease progression in diabetes patients using the popular Diabetes dataset. The goal is to understand the relationship between BMI and disease progression using a supervised learning model.

---

## 📁 Dataset

We used the **Diabetes dataset** available through Scikit-learn. It contains:

* **442 samples**
* **10 baseline features** (we used `bmi`)
* **Target**: A quantitative measure of disease progression after one year

---

## 🔍 Objective

To predict the diabetes progression score based on a patient’s BMI using:

* **Linear Regression model**
* **Train-Test Split**
* **Performance Evaluation (MAE, MSE, R² Score)**

---

## 🧪 Workflow

### 1. Data Loading

* Imported the Diabetes dataset via `sklearn.datasets`
* Converted to Pandas DataFrame for better handling

### 2. Feature Selection

* Chose **BMI** as the single independent feature (X)
* Target (`y`) is disease progression metric

### 3. Data Splitting

* Split into **80% training** and **20% testing**

  ```python
  X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=0.2, random_state=42)
  ```

### 4. Model Training

* Trained using `LinearRegression()` from `sklearn.linear_model`

### 5. Predictions & Evaluation

* Predictions made on the test set
* Evaluated using:

  * **Mean Absolute Error (MAE)**
  * **Mean Squared Error (MSE)**
  * **R² Score**

---

## 📈 Results

| Metric       | Value     |
| ------------ | --------- |
| **MAE**      | \~44.43   |
| **MSE**      | \~2900.17 |
| **R² Score** | \~0.38    |

**Insights from Visualization:**

* The scatter plot of actual vs predicted values showed a visible linear trend.
* However, prediction accuracy could improve with more features or advanced models.

---

## 📌 Key Learnings

* Linear Regression is simple yet effective for univariate predictions.
* R² Score of 0.38 indicates BMI alone is not sufficient for highly accurate predictions.
* Feature expansion or model tuning could enhance performance.

---

## 📚 Technologies Used

* Python
* Scikit-learn
* Pandas, NumPy
* Matplotlib, Seaborn
* Jupyter Notebook

---

## 🚀 How to Run

1. Clone this repo
2. Install dependencies

   ```
   pip install -r requirements.txt
   ```
3. Open the Jupyter Notebook:

   ```
   jupyter notebook LR.ipynb
   ```

---

## 🙌 Acknowledgements

Thanks to **Scikit-learn** for the dataset and tools used for building this model.

---

