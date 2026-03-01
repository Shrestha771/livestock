### Livestock Disease Prediction System

---

### Overview
This project aims to predict potential diseases in livestock using machine learning techniques.  
Early disease prediction helps in timely treatment, reduces economic loss, and improves livestock health management.

The system uses real-world livestock health data and applies supervised machine learning models to classify possible disease outcomes.

---

### Problem Statement
Livestock diseases are often diagnosed at later stages due to limited access to veterinary services and delayed symptom recognition.  
This project focuses on using data-driven methods to assist in early disease detection using machine learning.

---

### Tech Stack
- Programming Language: Python  
- Data Analysis: Pandas, NumPy  
- Machine Learning: Scikit-learn  
- Visualization: Matplotlib, Seaborn  
- Model Persistence: Pickle  

---

### Project Structure

ai_model/
│
├── data/
│   └── livestock_dataset.csv
│
├── models/
│   ├── label_encoder_animal.pkl
│   ├── label_encoder_breed.pkl
│   ├── label_encoder_disease.pkl
│   ├── label_encoder_product.pkl
│   └── livestock_disease_predictor.pkl
│
├── src/
│   ├── data_preprocessing.py
│   ├── model_training.py
│   ├── predict.py
│
└── main.py

---

### Dataset
The project uses a livestock health dataset containing symptom and production-related attributes.

- Data preprocessing was performed to handle missing values and inconsistencies  
- Categorical features were encoded using LabelEncoder  
- Encoders are saved inside the `models/` directory  
- Due to data usage constraints, the full dataset may not be publicly shared  

---

### Methodology
- Performed data cleaning and preprocessing  
- Conducted exploratory data analysis (EDA)  
- Selected key features relevant to disease prediction  
- Trained and evaluated machine learning models:
  - Logistic Regression  
  - Random Forest  
- Compared model performance and selected the best-performing model  
- Saved trained model and encoders for prediction  

---

### Results
The models demonstrated effective classification performance.  
Random Forest achieved higher accuracy compared to Logistic Regression, indicating strong capability in handling structured livestock health data.

The results show the feasibility of applying machine learning for early livestock disease detection.

---

### How to Run

1. Clone the repository:

git clone https://github.com/Shrestha771/livestock.git  
cd ai_model

2. Install dependencies:

pip install pandas numpy scikit-learn matplotlib seaborn  

3. Train the model:

python src/model_training.py  

4. Run prediction:

python src/predict.py  

5. Or execute full pipeline:

python main.py  

---

