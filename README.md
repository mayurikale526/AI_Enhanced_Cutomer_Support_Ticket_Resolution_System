# Automated Support Ticket Resolution System
This project is designed to automate the resolution of customer support tickets using advanced NLP techniques, vector databases, and integrations with third-party tools like Pinecone and Zapier. The system retrieves similar past issues, generates personalized responses, and integrates with email systems for seamless communication.
## Project Structure

###### Root Directory
1. *app/:* Contains the main pipeline notebook for the support ticket system. ( NOT UPDATED! )

2. *data/:* Contains datasets used for training and testing the system.
   helpdesk_customer_tickets (1).csv: Customer support tickets dataset.
   train-00000-of-00001-a5a7c6e4bb30b016.parquet: Training data in Parquet format.

3. *rough/:* Contains exploratory work and drafts for various components of the project.

   *-Analysis/:* Exploratory data analysis (EDA) notebooks and scripts.
   *-Sentiment Analysis/:* Sentiment analysis experiments and notebooks.
   *-Automated Response/:* Drafts and experiments for automated response generation.
   *Real Time Escalation/:* Work on real-time escalation systems.
   *Issue Prevention Dashboard/:* Work on dashboards for issue prevention.

4. README.md: This file, providing an overview of the project.



![Screenshot 2025-01-29 192819](https://github.com/user-attachments/assets/7f2b5a49-b89d-49d3-bb6d-0868278ec6e8)
## Features
#### 1. Automated Ticket Resolution:
  -Retrieves similar past issues using vector embeddings and Pinecone.
  -Generates personalized responses using OpenAI's GPT models.
  
##### 2. Email Integration:
  -Integrates with Zapier and ngrok for automated email responses.
  
##### 3. Multilingual Support:
  -Handles support tickets in multiple languages.

##### 4. Real-Time Escalation:
 -Identifies and escalates critical issues in real-time.

##### 5. Sentiment Analysis:
  -Analyzes customer sentiment to prioritize and personalize responses.

##### 6. Issue Prevention Dashboard:
  -Provides insights into common issues and trends to prevent future problems.

  
## Setup Instructions
#### Prerequisites
1. Python 3.10 or later.
2. Required Python libraries (install via pip):
pip install pandas numpy openai pinecone-client sentence-transformers transformers ngrok zapier

3. API keys for:
  -OpenAI
  -gspread
  -Pinecone
  -ngrok (if using local tunneling)
