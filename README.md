# warfarin-dosing-ml-tool-
End-to-end machine learning pipeline for predicting optimal Warfarin dosage using clinical and genetic data. Built using Python, scikit-learn, and Gradio for interactive prediction.

# 💊 Warfarin Dosing Prediction Tool

This project implements a complete **end-to-end machine learning pipeline** to predict optimal weekly **Warfarin** dosage for patients based on clinical and genetic data. Warfarin is a widely used anticoagulant, but incorrect dosing can cause serious complications. This tool aims to support clinicians with accurate dosage recommendations.

## 📌 Project Highlights

- ✅ Dataset: **International Warfarin Pharmacogenetics Consortium (IWPC)**
- 🛠️ Techniques: Data preprocessing, imputation, outlier detection, one-hot encoding
- 📊 Models Used: Linear Regression, Logistic Regression, Decision Tree, Random Forest, Gradient Boosting, MLP (Deep Learning)
- 🌐 Interactive UI: Built using **Gradio** for real-time predictions
- 📈 Metrics: 
  - Regression: RMSE = **12.07**, R² = **0.40**
  - Classification: Accuracy = **74.12%**, F1-Score = **0.7381**

## 📂 Project Structure

├── Final_Project.ipynb # Jupyter notebook with full ML pipeline
├── report/
│ └── Final Project 42 warfarin.pdf # Final project report
├── docs/
│ └── Final_project_code.pdf # Code documentation
├── README.md


## 📋 Key Features

- Handles missing values and outliers robustly
- Encodes categorical data and prepares clean features
- Trains and compares multiple models for classification and regression
- Deploys a simple Gradio web app for dose prediction

## 🧪 Test Cases (Gradio Output Examples)

- **Case 1**: 60-year-old Black male, 170 cm, 85 kg, genotype *1/*1 and G/G  
  → Predicted Dose: **51.69 mg/week**, Class: **High**

- **Case 2**: 52-year-old Asian female on Amiodarone, 170 cm, 47 kg, genotype *2/*3 and A/A  
  → Predicted Dose: **2.94 mg/week**, Class: **Low**

## 📈 Model Performance Summary

| Model                | Task         | Accuracy/F1 / RMSE | Notes                           |
|---------------------|--------------|---------------------|---------------------------------|
| Logistic Regression | Classification | 74.1% / 0.7381      | Best classification model       |
| Linear Regression   | Regression     | RMSE = 12.07        | Best regression model           |
| MLP Regressor       | Regression     | RMSE = 12.13        | Deep learning, similar results  |

## 🤝 Team Contributions

- **Ifthekar Hussain**: Data preprocessing, classification models, visualizations
- **Sri Vasista Talagampala**: Regression models, MLP, Gradio interface, final report

## 💻 How to Run

1. Clone this repo  
2. Open `Final_Project.ipynb` in Google Colab or Jupyter  
3. Install required packages (`pandas`, `scikit-learn`, `matplotlib`, `gradio`)  
4. Run all cells to see model predictions and launch Gradio app


## 🚀 Live Demo

🔗 Try the interactive Warfarin dose prediction tool here:  
👉 [Launch Gradio App](https://38418be05f8f61d359.gradio.live/)

> Enter patient info (age, weight, genotype, etc.) to get an instant dosage prediction and classification (High or Low).

   

## 📜 Disclaimer

This project is for educational purposes only and should not be used for real medical decisions. Always consult a healthcare professional.

