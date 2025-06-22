# Build Smart Agent AI-powered apps for Diet Planner using Streamlit, Gemini Pro 2.5, Google ADK, Vertex AI and BigQuery

In this tutorial, we'll create an intelligent diet planning web application that leverages generative AI, Google Cloud services, and Streamlit's simplicity. The app will generate personalized meal plans based on user biometrics and store data for future reference.

## Solution Overview :
- <b>Streamlit</b>: Frontend interface for user inputs
- <b>Gemini Pro 2.5 LLM model</b>: Generate diet plans via Vertex AI
- <b>Google Agent Development Kit</b>: Backend logic for plan generation
- <b>BigQuery</b>: Secure user data storage

## Key Features
- Biometric inputs: Weight, height, age, gender
- Personalized diet plan generation
- Historical data storage/retrieval
- Diet Plan can be download to save to your local computer
- Google Cloud integration

## Setup Instructions :
1. Google Cloud Setup
    - Create a GCP project and enable:
        - Vertex AI API
        - BigQuery API
    - Create service account with:
        - BigQuery User
        - BigQuery Data Editor
        - Vertex AI Service Agent
        - Vertex AI User
    - Generate and download JSON key
2. BigQuery Setup
   
   Create new Dataset : diet_planner_data
3. Installation
   - git clone this repo
    - Create python virtual env
    ```
    python -v venv .env
    ```
    - Activate new virtual env
    ```
    source .env/bin/activate
    ```
    - Install all python libraries in requirements.txt 
    ```
    pip install -r requirements.txt
    ```
    - Change value project_id, location and gcp_service_account in secrets.toml under folder .streamlit to your gcp account
4. Run locally
   
   Type command bellow to run streamlit apps
    ```
    streamlit run app.py
    ```

