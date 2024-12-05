# Flood Prediction System

## Project Overview
This project predicts the likelihood of floods based on monthly rainfall data and annual rainfall. By accurately predicting flood occurrences, we aim to improve disaster preparedness and resource allocation, ultimately minimizing damage and saving lives. The project utilizes machine learning and a user-friendly Tkinter-based GUI to make predictions accessible to non-technical users.

---

## Problem Statement
Floods are one of the most frequent and devastating natural disasters, leading to significant loss of life and property. Accurate flood prediction can help mitigate these risks by enabling timely intervention and better disaster management. The main objective of this project is to predict flood occurrences based on monthly rainfall and annual rainfall data using machine learning.

---

## Data Collection
The data used for this project was sourced from:
- **Kerala Rainfall Dataset**: A dataset containing monthly rainfall data and annual totals for flood prediction.  
- **Dataset Link**: [Kerala Rainfall Dataset on Kaggle](https://www.kaggle.com/code/mukulthakur177/flood-prediction-model)

---

## Methodology

### Data Wrangling
- Cleaned and preprocessed the dataset to handle missing values.
- Transformed the target variable (`FLOODS`) into a binary format (1 for "YES", 0 for "NO").
- Normalized the feature data using a Min-Max Scaler to ensure uniformity.

### Exploratory Data Analysis (EDA)
- Visualized monthly and annual rainfall distributions using histograms.
- Identified key rainfall months contributing to flood occurrences.
- Analyzed correlations between rainfall features and flood outcomes.

### Predictive Analysis
- Implemented a **Random Forest Classifier** to predict flood occurrences.
- Split the dataset into training (80%) and testing (20%) sets for model evaluation.
- Hyperparameter tuning was conducted to optimize model performance.
- Evaluated the model using metrics such as accuracy, recall, and ROC AUC scores.

---

## Key Results
- The **Random Forest Classifier** achieved the following performance metrics:
  - **Accuracy**: 87.5%
  - **Recall**: 92.31%
  - **ROC AUC Score**: 87.06%
- Monsoon months (**June, July, August, September**) and high annual rainfall were key predictors of floods.

---

## Visualizations
- **Histograms**: Displayed distributions of monthly rainfall.
- **Confusion Matrix**: Showed true positives, false positives, true negatives, and false negatives for model predictions.
- **ROC Curve**: Illustrated the model's ability to distinguish between flood and no-flood years.
- **Feature Importance Plot**: Highlighted the most influential rainfall features in flood prediction.

---

## How It Works
1. The user enters monthly rainfall data (January–December) and the total annual rainfall into the Tkinter GUI.
2. The input data is normalized and passed to the trained Random Forest Classifier.
3. The model predicts whether a flood is expected and displays the result along with the confidence percentage directly in the GUI.

---

## Future Enhancements
- Add options for uploading rainfall data from external files.
- Integrate additional data sources (e.g., river levels, soil moisture) for improved predictions.
- Build a web-based interface for broader accessibility.

---

## License
This project is licensed under the MIT License.

---

## References
- **Kerala Rainfall Dataset on Kaggle**: [Link](https://www.kaggle.com/code/mukulthakur177/flood-prediction-model)
- **Python Libraries**: NumPy, Pandas, Matplotlib, Seaborn, Scikit-learn, Tkinter
