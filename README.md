📩 Spam Message Classifier

A Machine Learning project that classifies SMS messages as Spam or Ham (Not Spam) using Natural Language Processing (NLP) techniques and multiple classification algorithms.

This project demonstrates the full machine learning pipeline, including:

Data preprocessing

Text vectorization

Model training

Model evaluation

Performance comparison

🚀 Features

Text preprocessing and cleaning

Feature extraction using:

Count Vectorizer

TF-IDF Vectorizer

Training multiple machine learning models

Performance comparison across models

Evaluation using accuracy and precision

🧠 Algorithms Used

The following machine learning algorithms were tested:

Multinomial Naive Bayes

Bernoulli Naive Bayes

Logistic Regression

Support Vector Machine (SVM)

Decision Tree

K-Nearest Neighbors (KNN)

Random Forest

AdaBoost

Bagging Classifier

Extra Trees Classifier

Gradient Boosting

XGBoost

🛠 Technologies Used

Python

Scikit-learn

Pandas

NumPy

NLTK

Matplotlib / Seaborn

XGBoost

📂 Project Structure
Spam-Classifier
│
├── SPAM Classifier.ipynb   # Main notebook
├── README.md               # Project documentation
├── dataset.csv             # SMS dataset
⚙️ Installation

Clone the repository:

git clone https://github.com/yourusername/spam-classifier.git

Install required libraries:

pip install -r requirements.txt

Or manually install:

pip install numpy pandas scikit-learn nltk xgboost matplotlib seaborn
📊 Machine Learning Pipeline
1️⃣ Data Cleaning

Remove unnecessary characters

Convert text to lowercase

Tokenization

Stopword removal

Stemming

2️⃣ Feature Extraction

Two methods were used:

Count Vectorizer

Converts text into a matrix of token counts.

TF-IDF Vectorizer

Weights words based on their importance in the dataset.

3️⃣ Train Test Split

Dataset divided into:

Training Data

Testing Data

Using:

train_test_split()
4️⃣ Model Training

Multiple models were trained and compared to find the best performing classifier.

Example:

mnb = MultinomialNB()
svc = SVC(kernel='sigmoid')
rfc = RandomForestClassifier()
5️⃣ Model Evaluation

Models were evaluated using:

Accuracy Score

Precision Score

Confusion Matrix

Spam detection focuses more on precision to avoid classifying normal messages as spam.

📈 Results

Among the tested models, Multinomial Naive Bayes with TF-IDF features performed very well for spam classification due to its effectiveness in text classification problems.

💡 Future Improvements

Deploy as a web app (Flask / Streamlit)

Use Deep Learning (LSTM / BERT)

Improve preprocessing pipeline

Build real-time spam detection API
