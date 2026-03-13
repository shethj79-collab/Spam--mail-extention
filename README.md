Spam Detection System using Machine Learning and Browser Extension
📝 Overview
This project aims to build an intelligent Spam Detection System that identifies and filters out spam emails using Machine Learning (ML). It combines a Python-based ML model with a browser extension to predict in real time whether an opened email is spam or not.

The system uses the Enron Email Dataset, performs data preprocessing and feature extraction using TF-IDF, and applies models such as SVM, Naive Bayes, and Random Forest to achieve high accuracy. The final model is deployed using Flask API, which connects seamlessly with a custom-built browser extension (HTML, CSS, JavaScript).

🚀 Key Features
Real-time spam detection in Gmail via browser extension
Lightweight Flask API for backend communication
Custom-trained ML model for accurate predictions
Clean and interactive UI in the extension popup
Focus on privacy — no data is stored or shared externally
Easy to integrate and expand
🧠 Technologies Used
Machine Learning & Backend:

Python
scikit-learn
NLTK
Flask
joblib
Frontend & Extension:

HTML
CSS
JavaScript
Chrome/Edge Extension APIs
Tools & Platforms:

Jupyter Notebook
Visual Studio Code
Google Chrome / Microsoft Edge
⚙️ How It Works
User opens an email in Gmail.
The browser extension extracts the email’s subject and message body.
Data is sent to the Flask API as JSON.
The API preprocesses the text, converts it into TF-IDF features, and runs the trained ML model.
The model predicts if the email is Spam (1) or Not Spam (0).
The result is sent back to the extension and displayed instantly.
🧩 Model Workflow
Data Collection – Enron Email Dataset
Data Cleaning & Preprocessing
Feature Extraction using TF-IDF
Model Training (SVM, NB, RF, Stacking)
Evaluation & Model Selection
Model Saving using joblib
Flask API Integration
Browser Extension Connection
🧪 Installation and Setup
1. Clone the Repository
git clone https://github.com/neelchau/Spam-mail-extension.git
2. Install Dependencies
3. Run Flask API
python app.py
4. Load Extension in Browser
Open Chrome/Edge → Go to Extensions → Manage Extensions
Enable Developer Mode
Click Load Unpacked → Select the extension/ folder
Open Gmail → Click “Check Mail” → See prediction
📊 Results
Model	Accuracy
Logistic Regression	95.8%
Naive Bayes	94.5%
Random Forest	96.1%
SVM	97.3%
Stacking Classifier	98.0%
🔒 Security Features
Local API – No third-party data sharing
Model processes only user-opened emails
Text data is not stored after prediction
🔮 Future Work
Integration with other email platforms (Outlook, Yahoo)
Add deep learning models (BERT, LSTM)
Online API deployment
User feedback loop for retraining
🏁 Conclusion
This project successfully integrates machine learning with real-time browser functionality to classify emails as spam or not. It demonstrates the use of data preprocessing, model training, API development, and browser automation — all in one complete system.
