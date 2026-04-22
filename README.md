# 🎓 Student Performance Prediction System

## 📌 Overview

This project aims to predict student academic performance using machine learning techniques. By analyzing various factors such as study time, family background, and past grades, the model provides insights into student outcomes.

The system follows a complete ML pipeline — from data preprocessing to model training and evaluation — making it a production-ready and scalable solution.

---

## 🚀 Features

* 📊 Data preprocessing and cleaning
* 🔍 Feature engineering (handling outliers & skewness)
* 🔄 Automated ML pipeline using `sklearn`
* 🤖 Model training using Random Forest Regressor
* 📈 Performance evaluation (R², MAE, MSE)
* 💾 Model saving and loading with `joblib`

---

## 🧠 Tech Stack

* Python 🐍
* Pandas & NumPy
* Scikit-learn
* Matplotlib & Seaborn
* Joblib

---

## 📂 Project Structure

```
├── Data_Preprocessing.ipynb        # Data cleaning & EDA
├── Final_preprocessed.ipynb       # Feature engineering & pipelines
├── testing_ml_models.ipynb        # Model training & evaluation
├── student-por.csv                # Dataset
├── model.pkl                      # Saved trained model
└── README.md                      # Project documentation
```

---

## ⚙️ Workflow

### 1️⃣ Data Preprocessing

* Removed irrelevant columns
* Checked missing values and duplicates
* Performed exploratory data analysis (EDA)

### 2️⃣ Feature Engineering

* Outlier handling using IQR method
* Log transformation for skewed data (`absences`)
* Encoding:

  * Binary → Label Encoding
  * Categorical → OneHot Encoding
* Scaling using StandardScaler

### 3️⃣ Pipeline Creation

Used `ColumnTransformer` and `Pipeline` to automate:

* Numeric processing
* Binary encoding
* Categorical encoding

### 4️⃣ Model Training

* Model: **Random Forest Regressor**
* Train-test split: 80-20
* Evaluated using:

  * R² Score
  * Mean Absolute Error (MAE)
  * Mean Squared Error (MSE)

---

## 📊 Model Performance

| Metric   | Value  |
| -------- | ------ |
| R² Score | 0.974  |      
| MAE      | 0.151  |
| RMSE     | 0.234  |

---

## 💡 Key Insights

* Previous grades (G1, G2) strongly influence final performance
* Absences impact performance but require transformation
* Socio-economic factors also contribute significantly

---

## ▶️ How to Run

### Step 1: Clone the repository

```bash
git clone https://github.com/your-username/student-performance-prediction.git
cd student-performance-prediction
```

### Step 2: Install dependencies

```bash
pip install -r requirements.txt
```

### Step 3: Run notebooks

Open Jupyter Notebook and execute:

* Data_Preprocessing.ipynb
* Final_preprocessed.ipynb
* testing_ml_models.ipynb

---

## 🔮 Future Improvements

* Deploy as a web application (Flask / FastAPI)
* Add deep learning models
* Improve feature selection
* Integrate real-time student input system


---

## 📜 License

This project is open-source and available under the MIT License.

---

## ⭐ Support

If you like this project, consider giving it a ⭐ on GitHub!
