# ANN-Classification-Churn
#  Customer Churn Prediction using ANN & Streamlit

This project implements an **Artificial Neural Network (ANN)** to predict whether a bank customer will churn (close their account) based on historical customer data.  
It features **data preprocessing**, **model training**, and a **Streamlit web app** for user-friendly predictions.

---

##  Features
- **ANN model** built using TensorFlow/Keras.
- Preprocessing steps: label encoding, one-hot encoding, scaling.
- Trained on **Bank Customer Churn** dataset (`Churn_Modelling.csv`).
- Interactive **Streamlit web app** with input sliders & dropdowns.
- Saves & loads:
  - Trained model (`model.h5`)
  - Encoders (`label_encoder_gender.pkl`, `onehot_encoder_geo.pkl`)
  - Scaler (`scaler.pkl`)

---

##  Project Structure
├── app.py # Streamlit app for real-time predictions
├── experiments.ipynb # Data preprocessing & model training
├── prediction.ipynb # Model loading & prediction test
├── Churn_Modelling.csv # Dataset
├── model.h5 # Trained ANN model
├── label_encoder_gender.pkl # Gender label encoder
├── onehot_encoder_geo.pkl # Geography one-hot encoder

---

##  Installation

1️ **Clone the Repository**
git clone https://github.com/yourusername/ann-customer-churn.git
cd ann-customer-churn

2️ **Create & Activate a Virtual Environment**

python -m venv venv
source venv/bin/activate # macOS/Linux
venv\Scripts\activate # Windows
├── scaler.pkl # StandardScaler for features
├── requirements.txt # Python dependencies
└── README.md # Project documentation

3️ **Install Dependencies**

---

##  Training the Model
- Open and run `experiments.ipynb`.
- Steps:
  1. Load dataset.
  2. Encode categorical variables.
  3. Scale features.
  4. Train ANN model.
  5. Save trained model & preprocessing objects.

---

##  Running the Streamlit App
After training (or using provided model files):
streamlit run app.py
Go to the link shown (e.g., `http://localhost:8501`) and enter customer parameters to see churn prediction results.

---

##  Example Prediction
**Input:**
- Geography: France  
- Gender: Male  
- Age: 40  
- Balance: 60000  
- Credit Score: 600  

**Output:**
Churn Probability: 0.42
The customer is not likely to churn.

---

##  Dataset
**Source:** Bank Customer Churn Modeling dataset (10,000 records).  
**Target Variable:** `Exited` (1 = churn, 0 = not churn).  
**Features:** Credit score, geography, gender, age, tenure, balance, products, card ownership, activity, salary.

---

##  Future Enhancements
- Add SHAP/feature importance explainability.
- Deploy online via Streamlit Cloud or Hugging Face Spaces.
- Support batch predictions via CSV upload.

---

## License
This project is licensed under the MIT License.

---

##  Author
Deepak Athresh R — Sofware Engineer Intern
Harshitha D G - AI Software Engineer Intern
