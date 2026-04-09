# SVM Optimization on Multi-Class Dataset

## 📌 Objective

The objective of this project is to optimize a Support Vector Machine (SVM) classifier on a multi-class dataset using iterative parameter tuning. The model is trained and evaluated across 10 different train-test splits, and the best parameters are selected based on classification accuracy.

---

## 📊 Dataset

We used the **Wine Quality Dataset** from the UCI Machine Learning Repository.

* Total samples: ~6500
* Features: 11 numerical attributes
* Target variable: Wine quality (multi-class classification)

The dataset is created by combining:

* Red wine dataset
* White wine dataset

---

## ⚙️ Methodology

### 1. Data Preprocessing

* Combined red and white wine datasets
* Performed feature scaling using StandardScaler
* Extracted features (X) and labels (y)

---

### 2. Data Splitting

* Dataset split into 70% training and 30% testing
* 10 different splits generated using different random seeds

---

### 3. SVM Optimization

For each split:

* Performed 100 iterations of parameter tuning

* Parameters optimized:

  * Kernel: linear, rbf, poly
  * C (regularization parameter)
  * Gamma

* Best parameters selected based on highest accuracy

---

### 4. Evaluation

* Recorded best accuracy for each sample
* Generated a comparative performance table
* Plotted convergence graph (accuracy vs iterations)

---

## 📈 Results

* Best Accuracy: XX.XX
* Average Accuracy: XX.XX
* Minimum Accuracy: XX.XX

The model performed best with the **RBF kernel** in most cases.

---

## 📉 Convergence Graph

The convergence graph shows how the accuracy improves over iterations for the best-performing sample.

*(Attach convergence.png here)*

---

## 📁 Project Structure

```
.
├── winequality-red.csv
├── winequality-white.csv
├── svm_results.csv
├── convergence.png
├── main.py
├── README.md
```

---

## ▶️ How to Run

1. Install required libraries:

```
pip install pandas scikit-learn matplotlib
```

2. Run the script:

```
python main.py
```

---

## 📌 Key Insights

* SVM performance is highly sensitive to kernel and C parameter
* RBF kernel generally provides better performance
* Feature scaling significantly improves results
* Randomized search helps in exploring parameter space efficiently

---

## 🚀 Future Improvements

* Use GridSearchCV or Bayesian Optimization
* Perform cross-validation instead of simple splits
* Tune additional hyperparameters
* Deploy the model using an API

---

## 👨‍💻 Author

Your Name

---

## 📎 GitHub

(Add your repository link here)

