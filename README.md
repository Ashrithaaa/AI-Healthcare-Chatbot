# AI-Healthcare-Chatbot


 📌 Project Overview
 
This project is an AI-powered Healthcare Chatbot that assists patients by:
- Providing appointment details.
- Retrieving prescription refill information.
- Offering sentiment-based responses using Azure AI NLP.

This chatbot, built using Flask, Azure AI Text Analytics, and Python, interacts with users via a REST API.



📌 Technologies Used

✅ Flask (for API Development)
✅ Azure AI Text Analytics (for NLP & Sentiment Analysis)
✅ Python (Backend Processing)
✅ JSON (Data Handling)



 📌 Installation & Setup
 
1️⃣ Install Dependencies
bash
pip install flask azure-ai-textanalytics


2️⃣ Update Azure API Credentials

- Go to [Azure Portal](https://portal.azure.com/)
- Create a Text Analytics Resource
- Retrieve API Key & Endpoint and update in `ai_healthcare_chatbot.py`:

python
AZURE_AI_KEY = "YOUR_AZURE_AI_KEY"
AZURE_AI_ENDPOINT = "YOUR_AZURE_AI_ENDPOINT"


3️⃣ Run the Chatbot Locally
bash
python ai_healthcare_chatbot.py


 📌 Usage & API Endpoints

Chatbot Interaction
✅ POST/chatbot

Request Body (JSON):
json
{
    "message": "What is my next appointment?",
    "patient_name": "John Doe"
}

Response (JSON):
json
{
    "response": "Your next appointment is on March 15, 2025 - 10:00 AM."
}



📌 Deployment Guide

Deploy to AWS Lambda (Serverless)

1️⃣ Install required packages:
bash
pip install serverless-wsgi flask

2️⃣ Deploy with AWS CLI:
bash
sls deploy




