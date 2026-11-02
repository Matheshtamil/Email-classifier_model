# 📧 Email Classification Using Machine Learning

## 📌 Project Overview

This project focuses on classifying emails into two categories: **Safe Email** and **Phishing Email** using Machine Learning.

Phishing emails are designed to trick users into revealing sensitive information, clicking malicious links, or downloading harmful attachments. This project uses Natural Language Processing (NLP) and the Multinomial Naive Bayes algorithm to identify potentially malicious emails based on their textual content.

## 🎯 Objectives

- Classify emails as Safe or Phishing.
- Perform data cleaning and preprocessing.
- Convert email text into numerical features using CountVectorizer.
- Train a Multinomial Naive Bayes classification model.
- Evaluate model performance using classification metrics.
- Predict the category of new email messages.

## 🛠️ Technologies Used

- **Programming Language:** Python
- **Libraries:**
  - Pandas
  - NumPy
  - Matplotlib
  - Seaborn
  - Scikit-learn
- **Machine Learning Algorithm:** Multinomial Naive Bayes
- **NLP Technique:** CountVectorizer

## 📂 Project Structure

```text
Email-Classification/
│
├── project_MAIL_CLASSIFIER.ipynb
├── Phishing_Email.csv
├── Cleaned_Phishing_Email.csv
├── requirements.txt
└── README.md
```

## 📊 Dataset Description

The dataset contains email messages and their corresponding categories.

**Dataset Features:**

| Column | Description |
|---|---|
| Email Text | Actual email content |
| Email Type | Email category (Safe Email / Phishing Email) |

**Dataset Distribution:**

| Category | Number of Records |
|---|---:|
| Safe Email | 10,978 |
| Phishing Email | 6,543 |
| **Total** | **17,521** |

## ⚙️ Project Workflow

### 1. Data Loading
Loaded the phishing email dataset using Pandas.

### 2. Data Cleaning
- Removed unnecessary index columns.
- Handled missing email content.
- Removed leading and trailing spaces.
- Removed empty email records.
- Removed duplicate emails.

### 3. Exploratory Data Analysis (EDA)
Visualized the distribution of Safe and Phishing emails using Seaborn and Matplotlib.

### 4. Feature and Target Separation
- **Input (X):** Email Text
- **Output (Y):** Email Type

### 5. Train-Test Split
Split the dataset into training and testing sets using an 80:20 ratio with stratified sampling.

### 6. Text Vectorization
Used `CountVectorizer` to convert email messages into numerical feature representations.

Configuration:
- Stop words: English
- Maximum features: 10,000

### 7. Model Training
Implemented the **Multinomial Naive Bayes** algorithm to learn patterns from the numerical email representations.

### 8. Model Evaluation
Evaluated the trained model using:
- Accuracy Score
- Precision
- Recall
- F1-Score
- Confusion Matrix

### 9. New Email Prediction
Tested the trained model with a new email message to predict whether it was Safe or Phishing.

## 📈 Model Performance

**Algorithm:** Multinomial Naive Bayes

<details>
<summary>Evaluation Results</summary>

| Metric | Score |
|---|---:|
| Accuracy | 96.95% |
| Precision (Phishing) | 97% |
| Recall (Phishing) | 95% |
| F1-Score (Phishing) | 96% |
| Precision (Safe) | 97% |
| Recall (Safe) | 98% |
| F1-Score (Safe) | 98% |

</details>

**Confusion Matrix:**

| | Predicted Phishing | Predicted Safe |
|---|---:|---:|
| Actual Phishing | 1,240 | 69 |
| Actual Safe | 38 | 2,158 |

<details>
<summary>Confusion Matrix Explanation</summary>

- True Positive: 1,240 phishing emails correctly identified.
- False Negative: 69 phishing emails incorrectly classified as safe.
- False Positive: 38 safe emails incorrectly classified as phishing.
- True Negative: 2,158 safe emails correctly identified.

</details>

## 🚀 How to Run the Project

**Step 1: Clone the repository**

```bash
git clone https://github.com/your-username/Email-Classification.git
```

**Step 2: Navigate to the project directory**

```bash
cd Email-Classification
```

**Step 3: Install the required libraries**

```bash
pip install pandas numpy matplotlib seaborn scikit-learn jupyter
```

**Step 4: Open Jupyter Notebook**

```bash
jupyter notebook
```

**Step 5:** Open `project_MAIL_CLASSIFIER.ipynb` and execute the cells sequentially.

Make sure `Phishing_Email.csv` is available in the project directory.

## 🔮 Future Improvements

- Implement additional algorithms such as Logistic Regression and Support Vector Machine (SVM).
- Experiment with TF-IDF vectorization.
- Apply advanced NLP techniques.
- Develop a web application using Flask or Streamlit.
- Improve phishing detection using deep learning techniques.

## 👨‍💻 Author

**Mathesh T**

B.Tech - Artificial Intelligence and Data Science

---

⭐ If you find this project useful, consider giving this repository a star!
