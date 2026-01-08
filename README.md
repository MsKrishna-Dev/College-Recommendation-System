# 🎓 College Recommendation System

A hybrid recommendation system that suggests Indian colleges based on user preferences such as **Course**, **City**, **Minimum Rating**, and **Maximum Fees**.  
The system combines **semantic similarity** using Sentence-BERT with **structured filtering** to generate accurate and practical recommendations.

---

## 📌 Problem Statement
Students often struggle to find suitable colleges due to differences in course naming, varying fees, and quality indicators. 
Traditional keyword-based search fails to capture the true intent of students. This project addresses the problem by using **semantic matching** and **hybrid scoring**.

---

## 🎯 Objectives
- Recommend colleges based on user-defined constraints
- Perform semantic matching of course preferences
- Balance relevance, quality, and affordability
- Provide ranked Top-N college recommendations

---

## ⚙️ Project Workflow
1. Load and preprocess college dataset  
2. Normalize numerical features (Rating, Fees)  
3. Generate course embeddings using Sentence-BERT  
4. Compute cosine similarity with user input  
5. Apply hybrid scoring (Similarity + Rating + Fees)  
6. Filter colleges based on user constraints  
7. Rank and return top recommendations  

---

## 🧠 Methodology
- **Sentence-BERT** is used to convert course names into embeddings
- **Cosine similarity** measures semantic relevance
- **MinMax scaling** normalizes ratings and fees
- **Hybrid score** combines multiple factors for ranking

---

## 🛠 Technologies Used
- Python
- Pandas
- NumPy
- Scikit-learn
- Sentence-BERT (SentenceTransformers)

---

## 📂 Project Structure
```
College-Recommendation-System/
│
├── data/
│ └── colleges.csv
│
├── notebooks/
│ └── college_recommendation.ipynb
│
├── requirements.txt
├── README.md
└── .gitignore
```

---

## ▶️ How to Run the Project
1. Clone the repository : git clone https://github.com/MsKrishna-Dev/College-Recommendation-System.git

2. Install dependencies : pip install -r requirements.txt

3. Open Jupyter Notebook

4. Run college_recommendation.ipynb

---

## 📊 Output

The system outputs a ranked list of colleges based on:
- Course relevance
- College rating
- Fee affordability
