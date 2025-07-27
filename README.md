🫀 Heart Disease Prediction using Machine Learning

This project aims to predict whether a person is at risk of heart disease using the UCI Heart Disease Dataset. It leverages a Logistic Regression model to analyze health indicators and classify patients based on risk. The notebook includes all essential steps from preprocessing to model evaluation.

📌 Objective

To build a binary classification model that can predict the presence or absence of heart disease in a patient based on clinical features.

📁 Dataset

- Source: [UCI Heart Disease Dataset](https://www.kaggle.com/datasets/ronitf/heart-disease-uci)
- Target: `1` (heart disease), `0` (no heart disease)
  
🔧 Tools & Libraries

- Python
- Pandas, NumPy
- Matplotlib, Seaborn
- Scikit-learn (`LogisticRegression`, `train_test_split`, `StandardScaler`)
- Evaluation: Accuracy, Confusion Matrix, ROC-AUC

🔍 Project Workflow

1. Data Preprocessing
- Loaded and explored the dataset
- Checked and confirmed no missing values
- Scaled numerical features using `StandardScaler`
- Split data into training and testing sets (80:20)
 2. Exploratory Data Analysis (EDA)
- Visualized class distribution
- Generated correlation heatmap
- Explored feature relationships using boxplots and countplots
3. Model Training
- Applied Logistic Regression with increased iterations (`max_iter=1000`)
- Trained model on scaled data
4. Model Evaluation
- Accuracy Score
- Confusion Matrix
- ROC Curve and AUC Score
5. Feature Importance
- Analyzed model coefficients to determine which features influence prediction most
  
📈 Results

- Accuracy: ~88%
- ROC AUC Score: High (indicating strong class separation)
- Key indicators affecting prediction included:
  - Chest pain type (`cp`)
  - Maximum heart rate (`thalach`)
  - ST depression (`oldpeak`)
  - Number of major vessels (`ca`)
    
📌 Conclusion

This project demonstrates how basic machine learning techniques can be applied to healthcare data for predictive diagnosis. Logistic Regression offers interpretable results and performs well for binary classification tasks like heart disease prediction.

🧠 Future Work

- Try advanced models like Random Forest, XGBoost
- Perform hyperparameter tuning
- Deploy as a web app using Streamlit or Flask
