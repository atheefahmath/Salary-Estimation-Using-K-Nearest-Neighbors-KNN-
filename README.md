# Salary Estimation Using K-Nearest Neighbors (KNN)

## 📌 Project Overview

This project predicts whether an employee's annual income is likely to be **above or below $50K** using the **K-Nearest Neighbors (KNN)** Machine Learning algorithm.

The model is trained on employee demographic and financial information such as age, education level, capital gain, and working hours per week. After training, the system can estimate the salary category of a new employee.

---

## 🚀 Features

* Data preprocessing and cleaning
* Feature scaling using StandardScaler
* KNN classification model
* Optimal K-value analysis using error rates
* Salary prediction for new employees
* Confusion matrix evaluation
* Accuracy score calculation

---

## 🛠️ Technologies Used

* Python
* NumPy
* Pandas
* Matplotlib
* Scikit-learn
* Google Colab

---

## 📂 Dataset

The project uses a salary dataset containing employee information and income categories.

### Input Features

* Age
* Education Level
* Capital Gain
* Hours Per Week

### Target Variable

* Income

  * 0 → Salary ≤ $50K
  * 1 → Salary > $50K

---

## ⚙️ Installation

### Clone the Repository

```bash
git clone https://github.com/your-username/salary-estimation-knn.git
cd salary-estimation-knn
```

### Install Required Libraries

```bash
pip install numpy pandas matplotlib scikit-learn
```

---

## ▶️ Running the Project

```bash
python salary_estimation_using_k_nearest_neighbor.py
```

Upload the dataset file (`salary.csv`) when prompted.

---

## 🧠 Machine Learning Workflow

### 1. Data Loading

The dataset is loaded using Pandas and inspected for structure and quality.

### 2. Data Encoding

Income labels are converted into numerical values:

```python
dataset['income'] = dataset['income'].map({
    '<=50K': 0,
    '>50K': 1
})
```

### 3. Data Splitting

The dataset is divided into:

* 75% Training Data
* 25% Testing Data

### 4. Feature Scaling

Standardization is performed using StandardScaler to improve model performance.

### 5. KNN Training

The model uses:

```python
KNeighborsClassifier(
    n_neighbors=2,
    metric='minkowski',
    p=2
)
```

---

## 📊 Model Evaluation

The project evaluates performance using:

* Mean Error Rate Graph
* Confusion Matrix
* Accuracy Score

Example Output:

```text
Confusion Matrix:
[[120  10]
 [ 15 105]]

Accuracy of the Model: 90.0%
```

---

## 📈 Finding the Best K Value

The project calculates prediction error for K values ranging from 1 to 39 and visualizes the results using Matplotlib.

This helps identify the optimal number of neighbors for classification.

---

## 🔍 Salary Prediction

After training, users can enter:

* Age
* Education Level
* Capital Gain
* Hours Per Week

The model predicts whether the employee's salary is likely to be:

* Above $50K
* Below or Equal to $50K

---

## 📚 Learning Outcomes

This project demonstrates:

* Classification using K-Nearest Neighbors
* Feature Scaling Techniques
* Hyperparameter Selection
* Model Evaluation
* Real-world Salary Prediction

---

## 🤝 Contributing

Contributions and suggestions are welcome.

Feel free to fork the repository and submit pull requests.

---

## 📄 License

This project is licensed under the MIT License.

---

## 👨‍💻 Author

Atheef Ahmath

Machine Learning & Data Science Enthusiast
