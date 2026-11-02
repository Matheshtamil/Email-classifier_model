# 📧 Email Classification Using Machine Learning

## 📌 Project Overview

This project uses Machine Learning and Natural Language Processing (NLP) to classify emails into two categories: **Safe Email** and **Phishing Email**.

The model analyzes email content and identifies potentially malicious phishing messages to help users recognize suspicious emails.

## 🎯 Objectives

- Identify phishing emails and distinguish them from safe emails.
- Perform text preprocessing and data cleaning.
- Convert text data into numerical features.
- Train a Machine Learning classification model.
- Evaluate model performance using classification metrics.
- Predict the category of new email messages.

## 🛠️ Technologies Used

- **Programming Language:** Python
- **Libraries:** Pandas, NumPy, Matplotlib, Seaborn
- **Machine Learning:** Scikit-learn
- **NLP:** CountVectorizer
- **Algorithm:** Multinomial Naive Bayes

## 📂 Project Structure

```text
Email-filter/
│
├── project_MAIL_CLASSIFIER.ipynb
├── README.md
├── requirements.txt
└── .gitignore
```

## 📊 Dataset

The dataset contains email messages categorized as Safe Email and Phishing Email.
## 📊 Dataset

The dataset used in this project is available on Kaggle.

[Download Phishing Email Dataset](https://www.kaggle.com/datasets/mathesh2004/phishing-email-dataset-and-its-cleaned-dataset)

Download the dataset and place the CSV file in the project directory before running the notebook.

## ⚙️ Project Workflow

1. **Data Loading:** Load the email dataset using Pandas.
2. **Data Cleaning:** Handle missing values, duplicates and unnecessary data.
3. **Exploratory Data Analysis:** Analyze email category distribution.
4. **Text Preprocessing:** Prepare email content for feature extraction.
5. **Feature Extraction:** Convert text into numerical features using CountVectorizer.
6. **Train-Test Split:** Divide the dataset into training and testing sets.
7. **Model Training:** Train the Multinomial Naive Bayes classifier.
8. **Model Evaluation:** Evaluate performance using accuracy, precision, recall and F1-score.
9. **Prediction:** Classify new email messages as Safe or Phishing.

## 🤖 Machine Learning Algorithm

**Multinomial Naive Bayes**

This algorithm is suitable for text classification tasks because it works with frequency-based text features.

## 📈 Model Performance

The model achieved approximately **96.95% accuracy** on the test dataset.

Evaluation metrics:
- Accuracy
- Precision
- Recall
- F1-Score
- Confusion Matrix

## 🚀 How to Run the Project

**1. Clone the repository**

```bash
git clone YOUR_GITHUB_REPOSITORY_LINK
```

**2. Navigate to the project directory**

```bash
cd Email-filter
```

**3. Install dependencies**

```bash
pip install -r requirements.txt
```

**4. Download the dataset**

Download the CSV dataset from the Hugging Face link provided above and place it inside the project directory.

**5. Run the Jupyter Notebook**

```bash
jupyter notebook
```

Open `project_MAIL_CLASSIFIER.ipynb` and execute the cells sequentially.

## 🔮 Future Improvements

- Experiment with TF-IDF vectorization.
- Compare multiple Machine Learning algorithms.
- Implement advanced NLP techniques.
- Develop a web application using Flask or Streamlit.
- Explore deep learning approaches for phishing detection.

## 👨‍💻 Author

**Mathesh T**

B.Tech - Artificial Intelligence and Data Science

---

⭐ If you find this project useful, don't forget to star the repository!
