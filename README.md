# 🧠 Explainable AI (XAI): Combining Neural Networks and Decision Trees

This repository presents a **hybrid AI approach** for enhancing model interpretability by integrating **Neural Networks** and **Decision Trees**. The research explores how decision trees can approximate the decision-making process of neural networks, thereby **improving explainability without sacrificing accuracy**.

---

## 📌 Table of Contents
1. [Project Overview](#-project-overview)  
2. [Repository Structure](#-repository-structure)  
3. [Data Description](#-data-description)  
4. [Methodology](#-methodology)  
5. [Usage Instructions](#-usage-instructions)  
6. [Requirements](#-requirements)  
7. [Results](#-results)  
8. [Contributing](#-contributing)  
9. [Author](#-author)  

---

## 🔍 Project Overview

- **Goal**: Develop a hybrid model that enhances the interpretability of **neural networks** using **decision trees**.  
- **Key Idea**: Use decision trees as **surrogate models** to approximate the decision-making of a trained neural network.  
- **Dataset**: Synthetic datasets with **linear, circular, elliptical, and square decision boundaries**.  
- **Models Used**: Multi-Layer Perceptron (MLP), Decision Trees, Linear SVM, Logistic Regression with Polynomial Features.  

### 🎯 Key Objectives
1. **Interpretability Enhancement**: Improve neural network explainability by integrating decision trees.  
2. **Feature Engineering**: Introduce derived features to enhance decision trees' ability to mimic neural networks.  
3. **Evaluation & Benchmarking**: Compare the hybrid approach with existing interpretability methods (e.g., SHAP, LIME).  

---

## 📂 Repository Structure
```
ExplainableAI/
├── notebooks/
│   ├── Explainable-AI-Final.ipynb  # Jupyter notebook for model training and evaluation
├── Explainable-AI-Final.pdf        # Research paper explaining methodology and findings
├── README.md                       # Project documentation
```

---

## 📊 Data Description

- **Dataset**: Synthetic classification datasets representing different decision boundaries.  
- **Feature Categories**:  
  - **Linear Decision Boundary**: Parallel to one axis.  
  - **Oblique Decision Boundary**: Diagonal separation between classes.  
  - **Circular Decision Boundary**: Classification based on radial distance.  
  - **Elliptical Decision Boundary**: More complex spatial decision surface.  
  - **Square Decision Boundary**: Classification based on a square decision region.  
- **Target Variable**: Binary classification (`Class 0` and `Class 1`).  

---

## ⚙️ Methodology

### **Data Preprocessing & Feature Engineering**
- **Synthetic Data Generation** → Custom datasets with different decision boundaries.  
- **Feature Engineering** → Introduce derived features (`Z`) to help decision trees approximate neural network boundaries.  

### **Machine Learning Models**
- **Neural Networks (MLP)** → Train on raw features to learn decision boundaries.  
- **Decision Trees** → Used as a **surrogate model** to approximate neural network decisions.  
- **Comparative Models**:  
  - **Linear SVM** → Benchmark for linear decision boundaries.  
  - **Logistic Regression (Polynomial Features)** → Compare against decision tree approximations.  

### **Evaluation Metrics**
- **Accuracy** → Measure classification performance.  
- **Precision & Recall** → Evaluate decision tree effectiveness in mimicking neural network predictions.  
- **Interpretability Score** → Compare rule complexity between decision trees and SHAP/LIME.  

---

## 🚀 Usage Instructions

### **1️⃣ Clone the Repository**
```bash
git clone https://github.com/sanyog-chavhan/ExplainableAI.git
cd ExplainableAI
```

### **2️⃣ Install Dependencies**
```bash
pip install -r requirements.txt
```

### **3️⃣ Run Jupyter Notebook**
```bash
jupyter notebook
```
- Open `notebooks/Explainable-AI-Final.ipynb`.  

### **4️⃣ Explore Results**
- The notebook contains **model training, evaluation, and visualizations**.  
- Refer to `Explainable-AI-Final.pdf` for an in-depth research breakdown.  

---

## 📦 Requirements

Below is a typical `requirements.txt`:

```txt
numpy
pandas
scikit-learn
matplotlib
seaborn
tensorflow
keras
jupyter
shap
lime
```

Ensure you have **Jupyter Notebook** installed to run the `.ipynb` file.

---

## 📈 Results

### **Model Performance Comparison**

| Model                  | Accuracy  |
|------------------------|----------|
| **Neural Network (MLP)**      | 96.72%   |
| **Decision Tree Approximation** | 92.84%   |
| **Linear SVM**         | 85.91%   |
| **Logistic Regression (Poly Features)** | 88.45%  |

### **Key Findings**
✅ **Neural Networks are highly accurate but lack transparency**.  
✅ **Decision Trees approximate neural network decision boundaries with 92.84% accuracy**.  
✅ **Feature Engineering significantly improves decision tree performance**.  
✅ **Hybrid approach balances accuracy with interpretability**.  

---

## 🤝 Contributing

1. **Fork** this repo.  
2. Create a new branch:
   ```bash
   git checkout -b feature/your-feature
   ```
3. Commit your changes:
   ```bash
   git commit -m "Add new model or fix bug"
   ```
4. Push to GitHub:
   ```bash
   git push origin feature/your-feature
   ```
5. Open a **Pull Request**.

---

## 👨‍💻 Author

**Sanyog Chavhan**  
Student - MSc Data Science
📩 **sanyogchavhan2016@gmail.com**  

For collaborations or inquiries, feel free to reach out! 🚀
