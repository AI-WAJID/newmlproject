# newmlproject
# Student Score Prediction Web App
A Flask web application that predicts student scores based on demographic and test preparation data using machine learning models (CatBoost, XGBoost).

Features
Simple web interface for input

Preprocessing and prediction pipeline

Custom error handling and logging

Ready for deployment (Render, Docker, etc.)

Tech Stack
Python, Flask

scikit-learn, CatBoost, XGBoost

Bootstrap 5 for frontend styling

Project Structure
text
newmlproject/
├── artifacts/              # Saved model & preprocessor
├── src/
│   ├── pipeline/           # Prediction pipeline classes
│   ├── utils.py            # Utility functions
│   ├── exception.py        # Custom exceptions
│   └── components/         # Data ingestion, transformation
├── templates/              # HTML templates (index.html, home.html)
├── app.py                  # Flask app entry-point
├── requirements.txt        # Project dependencies
├── Procfile                # For Render deployment
└── Dockerfile              # Optional Docker config
Setup & Run
Clone the repo:

text
git clone https://github.com/AI-WAJID/newmlproject.git
cd newmlproject
Create and activate a Python environment, then install dependencies:

text
pip install -r requirements.txt
Ensure artifacts/model.pkl and artifacts/preprocessor.pkl exist (generated from training).

Run the app:

text
python app.py
Open browser to http://localhost:5000/ and use the app.

Deployment Tips
Add a Procfile with:

text
web: gunicorn app:app
Use port configuration in app.py to listen on Render-assigned ports.

Use Docker for containerized deployment if desired.
