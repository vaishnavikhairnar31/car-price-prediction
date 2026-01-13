# 🚗 Car Price Prediction – Full-Stack Machine Learning Application

## 🔗 Live Project Links

- 🌐 **Streamlit Web App (Frontend)**  
  👉 https://car-price-prediction-fzmbdxbbhwzpc8hcdun67d.streamlit.app/
  
- ⚙️ **FastAPI Backend (Swagger Docs)**  
  👉 https://car-price-prediction-0f8s.onrender.com/docs

- 📂 **GitHub Repository**  
  👉 https://github.com/vaishnavikhairnar31/car-price-prediction

This project is a **full-stack machine learning application** that predicts the **selling price of second-hand cars** using real-world features such as year of purchase, fuel type, transmission, number of owners, and kilometers driven.

I built this project **end-to-end** to understand how a machine learning model is **trained, deployed as an API, and consumed by a frontend application** in a real-world setup.

---

## 📌 Problem Statement

Determining the correct price of a used car is challenging because many factors influence its value.  
This application provides a **data-driven price estimation** using historical car data and machine learning.

---

## 🧠 Project Overview

The project consists of **three main components**:

### 1️⃣ Machine Learning Layer
- Trained a **Random Forest Regressor** using Scikit-learn  
- Performed data preprocessing and one-hot encoding  
- Serialized the trained model for real-time predictions  

### 2️⃣ Backend – FastAPI
- Developed a REST API using **FastAPI**  
- Used **Pydantic** for request validation and type safety  
- Loaded the trained model and performed inference on incoming data  

### 3️⃣ Frontend – Streamlit
- Built an interactive UI using **Streamlit**  
- Collected user inputs and sent them to the backend API  
- Displayed predicted car prices instantly  

---

## ⚙️ Tech Stack

- **Python**
- **Pandas, NumPy**
- **Scikit-learn**
- **FastAPI**
- **Pydantic**
- **Streamlit**
- **Uvicorn**
- **Git & GitHub**

---

---

## 📁 Project Structure

car-price-prediction/                                                                                                                                                   
│                                                                                                                                                              
├── train.py # Model training script                                                                                                                                                         
├── main.py # FastAPI entry point                                                                                                                                                   
├── model.py # Model loading & prediction logic                                                                                                             
├── schema.py # Pydantic schemas                                                                                                                                                         
├── streamlit_app.py # Streamlit frontend                                                                                                                   
│                                                                                                                                                                     
├── cardekho_data.csv # Dataset                                                                                                                        
├── requirements.txt # Project dependencies                                                                                                                               
├── runtime.txt # Python version (deployment)                                                                                                               
├── .gitignore                                                                                                                                          


---

## 🧪 Machine Learning Details

- **Algorithm**: Random Forest Regressor  
- **Target Variable**: Selling Price  
- **Preprocessing**:
  - One-hot encoding for categorical features  
  - Feature alignment during inference to avoid mismatch  
- **Model Persistence**:
  - Model saved using `joblib` for efficient real-time predictions  

---

## 🚀 How to Run the Project Locally

### 1️⃣ Clone the Repository
```bash
git clone https://github.com/vaishnavikhairnar31/car-price-prediction.git
cd car-price-prediction
```
2️⃣ Create and Activate Virtual Environment                                                                                                                                          
python -m venv venv                                                                                                                                             
venv\Scripts\activate                                                                                                 
                                                                                                                                                                                 
3️⃣ Install Dependencies                                                                                                                                                     
pip install -r requirements.txt                                                                                                                                 
                                                                                                                                                                  
4️⃣ Train the Model (Optional)                                                                                                                                         
python train.py                                                                                                                                                                  
                                                                                                                                                                                                  
5️⃣ Start FastAPI Backend                                                                                                                                 
uvicorn main:app --reload                                                                                                                                    
                                                                                

FastAPI runs at:

http://127.0.0.1:8000

6️⃣ Start Streamlit Frontend                                                                                                 
streamlit run streamlit_app.py

📚 Key Learnings

Built a complete ML pipeline from training to deployment

Learned how to expose ML models using REST APIs

Ensured feature consistency between training and inference

Integrated backend APIs with frontend applications

Followed clean Git and GitHub workflows

