# Insurance Premium Prediction API using FastAPI 🚀

This project demonstrates an **end-to-end Machine Learning model deployment pipeline** using **FastAPI**.  
It covers everything from **model training** to **API-based inference** and finally **frontend consumption** using Streamlit.

The main goal of this project is to show **how a trained Machine Learning model can be served to users via an API**.

---

## 📌 Project Overview

In this project, we build an **Insurance Premium Prediction system** that classifies users into:

- **Low Premium**
- **Medium Premium**
- **High Premium**

based on their personal, lifestyle, and financial attributes.

The complete workflow includes:

1. Machine Learning model building  
2. Serving the model using FastAPI  
3. Consuming the API using a frontend (Streamlit)

---

## 🧠 Problem Statement

Insurance premium amounts depend on multiple factors such as:

- Age  
- Body metrics  
- Income  
- Lifestyle habits  
- Occupation  
- City category  

The objective is to predict **which premium category a user belongs to** using these inputs.

---

## 🧩 Tech Stack

- Python  
- FastAPI  
- Pydantic  
- Scikit-learn  
- Pandas & NumPy  
- Streamlit  
- Pickle  

---

## 🏗️ Project Architecture

User Input → Streamlit UI → FastAPI Endpoint → Feature Engineering → ML Model → JSON Response → UI Display

---

## 📁 Project Structure

```
├── app.py
├── front.py
├── model.pkl
├── requirements.txt
├── README.md
```

---

## 🧪 Machine Learning Model

- Algorithm: Random Forest Classifier  
- Dataset: Toy (synthetic) dataset  
- Target: Insurance Premium Category  

### Feature Engineering
- BMI  
- Age Group  
- Lifestyle Risk  
- City Tier  

⚠️ This model is for demonstration purposes only.

---

## 🔐 API Design

### Endpoint
POST /predict

### Sample Request
```json
{
  "age": 35,
  "weight": 79,
  "height": 1.72,
  "income_lpa": 10,
  "smoker": false,
  "city": "Gurgaon",
  "occupation": "government_job"
}
```

### Sample Response
```json
{
  "predicted_category": "Low"
}
```

---

## 🚀 Running the Project

### Install dependencies
```bash
pip install -r requirements.txt
```

### Run FastAPI
```bash
uvicorn app:app --reload
```

### Run Streamlit
```bash
streamlit run front.py
```

---

## 📌 Key Learnings

- ML model serving using FastAPI  
- POST-based inference APIs  
- Feature engineering inside APIs  
- API consumption using frontend  

---

## 🙌 Conclusion

This project showcases a complete ML deployment workflow and is ideal for learning FastAPI-based ML serving.

⭐ Star the repo if you found it helpful!
