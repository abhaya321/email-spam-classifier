📧 Email Spam Classifier

Project Description

This project detects whether an email is spam or ham (legitimate) using machine learning. It preprocesses email text with TF-IDF vectorization and classifies emails using Logistic Regression. It helps filter unwanted emails and improve inbox security.

Features

* Automatically classifies emails as spam or ham
* Text preprocessing and feature extraction with TF-IDF
* Uses Logistic Regression for binary classification
* Predicts new email messages as spam or ham

Dataset

* **Filename:** `mail_data.csv`
* **Columns:**

  * `Category` — Label for each email (spam or ham)
  * `Message` — The email text content
* Labels converted: spam → 0, ham → 1
* Dataset size: (include number of rows if known)

Technologies Used

* Python 3
* Pandas
* NumPy
* scikit-learn
* Jupyter Notebook

Usage

* Run all notebook cells to train and test the model
* Use the example code below to predict a new email:

```python
input_mail = ["Congratulations! You've won a free gift card."]
input_features = feature_extraction.transform(input_mail)
prediction = model.predict(input_features)

if prediction[0] == 1:
    print("Ham mail")
else:
    print("Spam mail")
```

---

How It Works

* Load and clean data (handle missing values, encode labels)
* Split data into training (80%) and testing (20%) sets
* Convert text emails into TF-IDF numeric features
* Train Logistic Regression model on training features
* Evaluate model accuracy on test data
* Predict spam or ham for new emails based on trained model

Results

* Training Accuracy: \~96%
* Test Accuracy: \~96%
  (Accuracy may vary depending on dataset and parameters)



