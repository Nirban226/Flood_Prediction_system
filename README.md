Flood Prediction System

A machine learning-based project that predicts the likelihood of floods based on monthly rainfall data and annual rainfall. This system uses a Random Forest Classifier to make predictions and provides a Tkinter-based GUI for user interaction.

Features

Predict flood occurrences based on rainfall inputs.
Provides confidence levels for predictions.
Simple and user-friendly GUI built with Tkinter.
Dataset

We used the Kerala Rainfall Dataset, which contains monthly rainfall data and annual totals for flood prediction.

Dataset: Kerala Rainfall Dataset on Kaggle
File name: Kerala.csv

Libraries Used

The project utilizes the following Python libraries:

NumPy: For numerical operations.
Pandas: For data manipulation and preprocessing.
Matplotlib: For visualizing data and results.
Seaborn: For enhanced data visualization.
Scikit-learn: For training the Random Forest Classifier and data scaling.
Tkinter: For building the graphical user interface.
To install the required libraries, run:

pip install numpy pandas matplotlib seaborn scikit-learn
How to Run

Clone the repository:
git clone https://github.com/yourusername/flood-prediction-system.git
Navigate to the project directory:
cd flood-prediction-system
Ensure the dataset (Kerala.csv) is in the same directory as the code.
Run the Python script:
python floods.ipynb
A GUI window will appear. Enter the rainfall data for each month and the annual rainfall, then click "Predict Flood" to see the prediction and confidence level.
Project Structure

floods.ipynb: Jupyter Notebook containing the model, prediction logic, and GUI.
Kerala.csv: Dataset used for training and prediction.
Model Details

Algorithm Used: Random Forest Classifier
Training-Test Split: 80% training, 20% testing
Performance Metrics:
Accuracy: 87.5%
Recall: 92.31%
ROC AUC Score: 87.06%
How It Works

The user enters monthly and annual rainfall data.
The input data is normalized using a Min-Max Scaler.
The Random Forest Classifier predicts whether a flood will occur and provides a confidence score.
The result is displayed directly in the GUI.
Future Enhancements

Add options to upload rainfall data from a file.
Include graphs for visualizing historical rainfall trends.
Support for multiple regions or datasets.
