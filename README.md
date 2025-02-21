echo "# Sentiment Analysis using BERT

This project implements a Sentiment Analysis API using \`nlptown/bert-base-multilingual-uncased-sentiment\` with Flask. It predicts whether a given text has a **Very Negative, Negative, Neutral, Positive, or Very Positive** sentiment.


## 🚀 Features
- Uses **BERT** for multilingual sentiment analysis.
- Flask API with a \`/predict\` endpoint.
- CORS enabled for easy frontend integration.


## 📌 Installation

### **1️⃣ Clone the Repository**
git clone https://github.com/rushikn/Sentiment-Analysis-BERT.git
cd Sentiment-Analysis/backend

### **2️⃣ Create a Virtual Environment**
python -m venv venv
source venv/bin/activate  # For Linux/macOS
venv\Scripts\activate      # For Windows

### **3️⃣ Install Dependencies**
pip install -r requirements.txt


## ▶️ Running the Server
python server.py
The server will start at **\`http://127.0.0.1:5000\`**.


## 📡 API Usage

### **Endpoint:**  
\`POST /predict\`

### **Request Format:**
{
  \"text\": \"Amazing service! I loved it.\"
}

### **Response Format:**
{
  \"sentiment\": \"Very Positive\",
  \"confidence\": 0.97
}


## 🛠 Testing the API

You can test the API using **Postman**, **cURL**, or Python.

### **Using Python (requests)**
import requests

url = \"http://127.0.0.1:5000/predict\"
data = {\"text\": \"Absolutely loved this product! The quality exceeded my expectations.\"}

response = requests.post(url, json=data)
print(response.json())
## 🛠 Author
Developed by rushikn 
GitHub: [@rushikn](https://github.com/rushikn)
