🩺 Multi-Disease Prediction System
📌 Overview

The Multi-Disease Prediction System is a machine learning-based project that predicts the likelihood of several chronic diseases, including:

Diabetes

Heart Disease

Kidney Disease

Liver Disease

Hypertension

Thyroid Disorder

Cancer

This project provides a unified interface where users can input their medical data and receive predictions for multiple diseases simultaneously.

🚀 Features

🔹 Multiple Models: Pre-trained ML models for each disease.

🔹 Unified Input: Supports both full feature names and abbreviations.

🔹 Flexible Age Handling: A single Age field is automatically mapped across all models.

🔹 Interactive CLI / Notebook: Easy-to-use input system.

🔹 Extensible: New disease models can be integrated with minimal changes.

🛠️ Tech Stack

Language: Python 3

Frameworks/Libraries:

Scikit-learn (ML models)

Pandas, NumPy (data preprocessing)

Jupyter Notebook (development & testing)

📂 Project Structure
healthy.ipynb        # Main notebook (training & prediction workflow)
models/              # Pre-trained ML models (saved .pkl files)
data/                # Dataset files (CSV/Excel)
utils/               # Helper functions (feature mapping, input handling)
README.md            # Project documentation

⚙️ How It Works

User provides medical input data (either full names or short aliases).

The system maps inputs using a smart_rename function.

Each disease model processes the relevant features.

Predictions are returned as “Positive / Negative” (with probability score if available).

▶️ Usage

Clone the repository:

git clone https://github.com/your-username/multi-disease-prediction.git
cd multi-disease-prediction


Install dependencies:

pip install -r requirements.txt


Run the notebook:

jupyter notebook healthy.ipynb


Enter patient details and run the prediction cells.

📊 Example Input
user_input = {
    "Age": 45,
    "Glucose": 130,
    "BloodPressure": 85,
    "BMI": 29.5,
    "Cholesterol": 220
}

✅ Example Output
Diabetes: Positive (78%)
Heart Disease: Negative (15%)
Kidney Disease: Negative (10%)
Liver Disease: Positive (65%)

🔮 Future Improvements

Web app interface using Streamlit / Flask

Integration with wearable devices (IoT health data)

Explainable AI (feature importance visualization)
