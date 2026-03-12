# 📩 Spam Message Classifier

A Machine Learning project that classifies SMS messages as **Spam** or **Ham (Not Spam)** using **Natural Language Processing (NLP)** techniques and multiple classification algorithms.

This project demonstrates the **complete machine learning pipeline**, including:

* Data preprocessing
* Text vectorization
* Model training
* Model evaluation
* Performance comparison

---

# 🚀 Features

* Text preprocessing and cleaning
* Feature extraction using:

  * Count Vectorizer
  * TF-IDF Vectorizer
* Training multiple machine learning models
* Performance comparison across models
* Evaluation using **accuracy and precision**

---

# 🧠 Algorithms Used

The following machine learning algorithms were tested:

* Multinomial Naive Bayes
* Bernoulli Naive Bayes
* Logistic Regression
* Support Vector Machine (SVM)
* Decision Tree
* K-Nearest Neighbors (KNN)
* Random Forest
* AdaBoost
* Bagging Classifier
* Extra Trees Classifier
* Gradient Boosting
* XGBoost

---

# 🛠 Technologies Used

* Python
* Scikit-learn
* Pandas
* NumPy
* NLTK
* Matplotlib
* Seaborn
* XGBoost

---

# 📂 Project Structure

```
Spam-Classifier
│
├── SPAM Classifier.ipynb   # Main notebook containing full ML workflow
├── dataset.csv             # SMS spam dataset
├── README.md               # Project documentation
```

---

# ⚙️ Installation

### Clone the Repository

```
git clone https://github.com/yourusername/spam-classifier.git
```

### Navigate to Project Folder

```
cd spam-classifier
```

### Install Required Libraries

Using requirements file:

```
pip install -r requirements.txt
```

Or install manually:

```
pip install numpy pandas scikit-learn nltk xgboost matplotlib seaborn
```

---

# 📊 Machine Learning Pipeline

## 1️⃣ Data Cleaning

The dataset undergoes several preprocessing steps:

* Remove special characters and punctuation
* Convert all text to lowercase
* Tokenization
* Stopword removal
* Stemming

These steps help reduce noise and improve model performance.

---

## 2️⃣ Feature Extraction

Text data must be converted into numerical format for machine learning models.

Two vectorization techniques were used:

### Count Vectorizer

Transforms text into a matrix of token counts.

### TF-IDF Vectorizer

TF-IDF assigns importance weights to words based on how frequently they appear across documents.

This helps highlight important words while reducing the influence of common words.

---

## 3️⃣ Train-Test Split

The dataset is divided into **training** and **testing** sets using:

```
train_test_split()
```

Training data is used to train the models while testing data evaluates their performance.

---

## 4️⃣ Model Training

Multiple machine learning models were trained to compare performance.

Example:

```
mnb = MultinomialNB()
svc = SVC(kernel='sigmoid')
rfc = RandomForestClassifier()
```

Each model learns patterns in the dataset to classify messages as **Spam or Ham**.

---

## 5️⃣ Model Evaluation

Models were evaluated using the following metrics:

* Accuracy Score
* Precision Score
* Confusion Matrix

In spam detection systems, **precision is especially important** because misclassifying normal messages as spam can negatively affect users.

---

# 📈 Results

Among all tested models, **Multinomial Naive Bayes with TF-IDF features performed the best**.

Naive Bayes models are particularly effective for text classification tasks because they handle high-dimensional sparse data efficiently.

---

# 💡 Future Improvements

Possible improvements for this project include:

* Deploying the model as a **web application (Flask or Streamlit)**
* Implementing **Deep Learning models such as LSTM or BERT**
* Improving the text preprocessing pipeline
* Creating a **real-time spam detection API**
* Adding model performance dashboards

---
