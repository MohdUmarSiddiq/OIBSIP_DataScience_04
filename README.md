# 📧 Email Spam Detection  

## 🌟 Overview  
This project focuses on detecting spam emails using machine learning and Natural Language Processing (NLP) techniques. The goal is to classify emails as either **spam** or **non-spam** based on their content.  

---

## 📊 Dataset  
The dataset used is **`spam.csv`**, which contains two columns:  
- **Category**: Labels indicating if the email is "spam" or "ham" (non-spam).  
- **Message**: The email text content.  

---

## 🔧 Steps Involved  

### 1️⃣ **Data Loading and Exploration**  
- 📥 Loaded the dataset using pandas.  
- 🔍 Explored the dataset for missing values, data imbalance, and text properties.  
- 📊 Visualized the distribution of spam and non-spam emails to understand the dataset better.  

---

### 2️⃣ **Data Preprocessing**  
- ✅ Converted text data to lowercase to ensure uniformity.  
- 🛑 Removed numbers, special characters, and punctuations from the text.  
- 🧹 Cleaned unnecessary spaces and standardized text.  
- ✂️ Tokenized the text into individual words and removed common stop words like "is," "and," etc.  
- 🌟 Performed **stemming** to reduce words to their root forms (e.g., "running" → "run").  

---

### 3️⃣ **Feature Extraction**  
- 📚 Transformed textual data into numerical vectors using:  
  - **Bag of Words (BoW)**  
  - **TF-IDF (Term Frequency-Inverse Document Frequency)**  

---

### 4️⃣ **Model Training**  
The following machine learning models were implemented:  
- 🤖 **Naïve Bayes**: A simple yet powerful algorithm for text classification.  
- 🧮 **Logistic Regression**: For probabilistic classification of emails.  
- 🌳 **Random Forest Classifier**: To improve classification accuracy by combining multiple decision trees.  

---

### 5️⃣ **Model Evaluation**  
- 📏 Evaluated the models using performance metrics such as:  
  - **Accuracy**  
  - **Precision**  
  - **Recall**  
  - **F1-Score**  

---

### 6️⃣ **Model Saving**  
- 💾 The trained model was saved using **Pickle** for later use in predictions. The saved model file is named **`spam_detection_model.pkl`**.  

---

### 7️⃣ **Deployment and Prediction**  
- 🖥️ Built a simple interface for predicting whether a given email is spam or not.  
- ✨ Used the trained model to classify new emails.  

---

## 🏆 Results  
- The **Naïve Bayes** model emerged as the most efficient algorithm with high precision and recall, making it the best choice for spam detection.  

---

## 🛠️ Requirements  
- **Python** (3.7 or above)  
- Libraries:  
  - pandas  
  - numpy  
  - sklearn  
  - nltk  

Install the necessary libraries using:  
```bash
pip install -r requirements.txt
```

## 🚀 How to Run the Project
1. 🖱️ Clone the repository to your local machine.
2. 📥 Load the dataset (spam.csv) into the appropriate directory.
3. 📦 Ensure the required libraries are installed using the command above.
4. ▶️ Run the Jupyter Notebook Email Spam Detection.ipynb to explore and execute the project step by step.
5. 📨 Use the saved model (spam_detection_model.pkl) for predictions on new email data.

## 🌍 Future Scope
Incorporate more advanced NLP techniques like word embeddings for better contextual understanding.

Expand the dataset to include more diverse email samples for enhanced model generalization.

Deploy the model as a web application for real-time spam email detection.
