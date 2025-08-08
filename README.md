# Bank FAQ Chatbot

A simple AI-powered chatbot built using **Streamlit** and **scikit-learn** that answers banking-related questions. It uses a Support Vector Machine (SVM) model trained on a dataset of frequently asked questions to predict the most relevant answer based on user input.

---

## Features

- Trained on a custom banking FAQ dataset (`BankFAQs.csv`)
- Uses `CountVectorizer` and `SVM` for text classification
- Matches user queries to the most similar question and provides an accurate answer
- Interactive and user-friendly UI built with Streamlit

---

## Installation

### 1.Clone the repository:
   ```bash
   git clone https://github.com/Gowthami970/Bank-FAQ-Chatbot.git
   cd Bank-FAQ-Chatbot
```

### 2.Create and activate a virtual environment (optional but recommended):
```bash
python -m venv myenv
# Windows
myenv\Scripts\activate
# macOS/Linux
source myenv/bin/activate
```

### 3.Install dependencies:
```bash
pip install -r requirements.txt
```

### Usage
Run the Streamlit app with:
```bash
streamlit run app.py
```
This will open the chatbot in your default browser at http://localhost:8501.

### Dataset
The chatbot is trained on BankFAQs.csv, which contains banking-related questions, their categories (classes), and answers.

### How it works
1.User enters a banking question.
2.The question is transformed into a vector using CountVectorizer.
3.The SVM model predicts the question’s class.
4.The app finds the most similar question in the predicted class and displays the corresponding answer.

### Technologies Used
Python
Streamlit
Pandas
Scikit-learn (SVM, CountVectorizer)
