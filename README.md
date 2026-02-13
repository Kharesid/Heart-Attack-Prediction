# Heart Attack Risk Prediction System

This project is a Machine Learning–based Heart Attack Risk Prediction application.
It uses a FastAPI backend to serve the trained ML model and a Streamlit frontend
to provide a simple and user-friendly interface.

---

## Project Description

The application predicts whether a person is at risk of a heart attack based on
medical parameters such as age, blood pressure, cholesterol level, heart rate,
and other clinical factors.

The system is divided into two parts:
- FastAPI Backend: Handles model loading, preprocessing, and prediction
- Streamlit Frontend: Collects user input and displays prediction results

---

## Project Structure

Heart_attack_prediction/
│
├── HD_API.py               # FastAPI backend API
├── app.py                  # Streamlit frontend application
├── HeartAprediction.ipynb  # Model training and experimentation notebook
└── README.md               # Project documentation

---

## Technologies Used

- Python
- FastAPI
- Streamlit
- Scikit-learn
- Pandas
- NumPy
- Uvicorn

---

## How to Run the Project

### Step 1: Create and Activate Virtual Environment

python -m venv .venv
.venv\Scripts\activate

---

### Step 2: Install Dependencies

pip install fastapi uvicorn streamlit scikit-learn pandas numpy requests

---

### Step 3: Run FastAPI Backend

uvicorn HD_API:heart_p_app --reload

The API will be available at:
http://127.0.0.1:8000

Swagger documentation:
http://127.0.0.1:8000/docs

---

### Step 4: Run Streamlit Frontend

Open a new terminal and run:

streamlit run app.py

The application will open automatically in your browser.

---

## Application Workflow

1. User enters health-related details in the Streamlit UI
2. Streamlit sends the data to the FastAPI /predict endpoint
3. FastAPI processes the input and runs the ML model
4. Prediction result is returned to Streamlit
5. The result is displayed as Low Risk or High Risk

---

## Prediction Output

- 0 : Low Risk of Heart Attack
- 1 : High Risk of Heart Attack

Note: This application is for educational purposes only and should not be used
as a substitute for professional medical advice.

---

## Author

Siddharth Khare 
Aspiring Data Scientist / Machine Learning Engineer

GitHub: https://github.com/Kharesid
