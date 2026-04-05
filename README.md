# Micro Project: Student Career Path Prediction using ANN 🎓

This repository contains the code and dataset for our Artificial Intelligence and Machine Learning (AIML) Micro-Project. The goal of this project is to predict a student's most likely future career path based on their academic performance, technical skills, and extracurricular activities using an Artificial Neural Network (ANN).

## 📂 Repository Contents
* **`Micro_Project.ipynb`**: The main Google Colab Jupyter Notebook containing the full data preprocessing pipeline, exploratory data analysis (EDA), and the ANN model architecture.
* **`cs_students.csv`**: The dataset containing numerical and categorical features of students (e.g., GPA, Coding Skills, Projects, etc.) used to train the model.
* **`career_model.keras`**: The saved weights of the fully trained neural network (generated after running the code).

## 🧠 Model Architecture & Machine Learning Techniques
We built a Multi-Layer Perceptron (MLP) using **TensorFlow/Keras**. To ensure high accuracy and real-world applicability, the project implements several advanced techniques:
* **Handling Class Imbalance:** Utilized `compute_class_weight='balanced'` to ensure the model accurately predicts rare, high-tier careers without simply defaulting to the majority class.
* **Regularization:** Applied **Dropout layers** and **L2 Kernel Regularization** to prevent the neural network from overfitting to the training data.
* **Robust Preprocessing:** Handled missing values (mean/mode imputation), applied `StandardScaler` for feature scaling, and used One-Hot Encoding with alignment to safely pass categorical data into the neural network without data leakage.

## 📊 Evaluation Metrics
The model is evaluated using:
* Overall Accuracy (Training vs. Testing)
* Precision, Recall, and F1-Scores for each individual career path
* A visual **Confusion Matrix** to track exact classification predictions

## 🛠️ Technologies & Libraries Used
* **Deep Learning:** TensorFlow, Keras
* **Machine Learning:** scikit-learn (Data splitting, Scaling, Metrics)
* **Data Manipulation:** pandas, NumPy
* **Data Visualization:** Matplotlib, Seaborn

## 🚀 How to Run the Project
1. Clone this repository or open the files directly on GitHub.
2. Open `Micro_Project.ipynb` using **Google Colab** (click the "Open in Colab" button if using a browser extension, or download and upload it to your Colab workspace).
3. Important: Ensure the `cs_students.csv` dataset is uploaded directly into your Colab session folder before running the code.
4. Run all cells to train the model and generate the evaluation graphs!
