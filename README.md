# url-phishing
# URL Phishing Detection using Machine Learning

## 📌 Project Overview
This project implements a machine learning model to detect phishing websites based on URL and domain-based features.

The model is trained using the UCI Phishing Website Dataset and classifies websites as:

- 0 → Legitimate
- 1 → Phishing

---

## 📊 Dataset Information

- Dataset: UCI Phishing Website Dataset
- Total Instances: 11,055
- Total Features: 30
- Target Variable: Result

Each instance represents one website described using 30 engineered URL, domain, and security features.

---

## 🧠 Model Used

### 🌳 Decision Tree (CART)
- Type: Classification Tree
- Criterion: Gini Impurity
- Train/Test Split: 80/20 (Stratified)
- Accuracy Achieved: ~97%

---

## ⚙️ Project Workflow

1. Load dataset
2. Data cleaning (remove ID column)
3. Convert labels (-1 → 1 phishing, 1 → 0 legitimate)
4. Train-test split
5. Train Decision Tree classifier
6. Evaluate model performance
7. Test on custom URLs using feature extraction

---

## 🔎 Feature Categories

The 30 features include:

- URL structure features
- SSL security features
- Domain registration features
- DNS record features
- Web traffic features
- Page rank & Google index
- Statistical and reputation indicators

---

## 📈 Model Performance

Precision, Recall and F1-score are balanced for both classes.

Accuracy: ~97%

This indicates strong performance on structured phishing detection data.

---

## 🚀 How to Run

1. Install dependencies:
   pip install pandas scikit-learn kagglehub

2. Run the notebook or Python script.
3. Train the model.
4. Use the extract_features() function to test custom URLs.

---

## ⚠️ Note

The simplified feature extractor included in this project demonstrates structural URL features only.

For real-world deployment, additional feature extraction such as:
- WHOIS lookup
- DNS validation
- PageRank analysis
- Google index check

would be required.

---

## 📌 Future Improvements

- Implement full feature extraction pipeline
- Compare with SVM and Random Forest
- Build web-based phishing detection app
- Add raw URL NLP-based model

---

## 👤 Author
Sanju

---

## 📄 License
This project is for educational purposes.
