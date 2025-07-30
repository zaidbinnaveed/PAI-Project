🧠 Stroke Prediction & Analysis Web App

📌 Project Overview

This project is a Flask-based web application that allows users to upload health datasets (CSV format) and get statistical analysis, data visualizations, and stroke prediction results using machine learning models like SVM and Random Forest.

It combines data preprocessing, EDA, ML model training, and interactive visualization in a seamless web interface, making it a valuable tool for healthcare analytics, academic learning, or machine learning experimentation.

🎯 Objectives

Predict the likelihood of stroke based on health attributes.

Perform statistical analysis and EDA on uploaded datasets.

Train and evaluate machine learning models.

Visualize patterns and correlations that may contribute to stroke prediction.

Provide results through a clean, user-friendly web interface.

🛠️ Technologies Used

Layer	Tools & Libraries
Frontend	HTML, Jinja2 Templates
Backend	Python, Flask
ML/EDA	pandas, seaborn, matplotlib, scikit-learn, imblearn
Deployment	Localhost (Flask Dev Server)

🧩 Features

🔹 Data Upload & Preprocessing
Accepts CSV input from the user

Handles missing values (e.g., BMI)

Encodes categorical features using One-Hot Encoding

Converts negative values to absolute (e.g., age, BMI)

🔹 Statistical Analysis

Calculates:

Mean, Median, Mode for age, BMI, glucose

Standard deviation

Correlation matrix

🔹 Visualizations (Rendered in Web App)

Pie chart of stroke distribution

Scatter plot (Age vs. Glucose Level)

Boxplot & violin plot for BMI

Heatmap of correlations

Age histogram

Gender & work type distributions

🔹 Machine Learning Models

Support Vector Machine (SVM):

RBF Kernel, balanced class weights

Random Forest Classifier:

Trained with SMOTE (to handle class imbalance)

Both models provide:

Accuracy Score

Classification Report (Precision, Recall, F1-Score)

🖥️ How It Works

Start the Flask App:

bash
Copy
Edit
python app.py
Navigate to Web Browser:

cpp
Copy
Edit
http://127.0.0.1:5000/
Upload Dataset:

Must be a CSV with features like age, bmi, avg_glucose_level, etc.

See Results:

View real-time analytics, charts, and ML model evaluations.

📊 Sample Output

Accuracy (SVM): ~85% (varies with dataset)

Accuracy (Random Forest): ~90% (after SMOTE)

Visuals: Embedded in result page as base64 PNGs

📌 Requirements

Install dependencies via pip:

bash
Copy
Edit
pip install flask pandas matplotlib seaborn scikit-learn imbalanced-learn
⚠️ Known Limitations

Only supports datasets with specific stroke-related features

No persistent model saving (trained per session)

Not deployed on cloud (runs on localhost)

Assumes specific column names (e.g., stroke, bmi, age, etc.)

🔮 Future Improvements

✅ Add file validation and dynamic feature detection

✅ Improve UI/UX with Bootstrap or React

🚀 Deploy on Heroku or Render

🧠 Add more ML models (e.g., XGBoost, Logistic Regression)

🧾 Include SHAP or LIME for model interpretability

🙋‍♂️ Author

Zaid Bin Naveed

Aspiring Data Scientist | Python Developer
