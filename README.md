# Diabetes Prediction using Support Vector Machine

This project aims to build a predictive model for diabetes using the PIMA Diabetes dataset. The model uses a Support Vector Machine (SVM) classifier with a linear kernel to classify individuals as diabetic or non-diabetic based on various health-related features.

## Table of Contents
- [Introduction](#introduction)
- [Dataset](#dataset)
- [Installation](#installation)
- [Usage](#usage)
- [Model Training and Evaluation](#model-training-and-evaluation)
- [Making Predictions](#making-predictions)
- [Results](#results)
- [Contributing](#contributing)
- [License](#license)
- [Acknowledgements](#acknowledgements)

## Introduction
This project aims to build a predictive model to classify individuals as diabetic or non-diabetic based on various medical attributes. The model is trained using the PIMA Indians Diabetes Database and leverages a Support Vector Machine (SVM) classifier for prediction.

## Dataset
The dataset used for this project is the PIMA Indians Diabetes Database, which is publicly available.

The dataset consists of the following features:

- Pregnancies: Number of times pregnant
- Glucose: Plasma glucose concentration after 2 hours in an oral glucose tolerance test
- BloodPressure: Diastolic blood pressure (mm Hg)
- SkinThickness: Triceps skinfold thickness (mm)
- Insulin: 2-Hour serum insulin (mu U/ml)
- BMI: Body mass index (weight in kg/(height in m)^2)
- DiabetesPedigreeFunction: Diabetes pedigree function
- Age: Age (years)
- Outcome: Class variable (0: non-diabetic, 1: diabetic)

## Installation
To run this project, you need to have Python installed along with the following libraries:
- numpy
- pandas
- scikit-learn

You can install the required libraries using:
`pip install numpy pandas scikit-learn`  

## Usage
- Clone the repository:  
`git clone https://github.com/your-username/diabetes-prediction.git`  
`cd diabetes-prediction`  
- Ensure the diabetes.csv file is in the data directory.

- Run the Jupyter notebook for exploratory data analysis and model building:  
`jupyter notebook notebooks/diabetes_prediction.ipynb`
- Alternatively, run the main Python script:  
`python src/diabetes_prediction.py`
## Model Training and Evaluation
The model is trained using a Support Vector Machine (SVM) with a linear kernel. The training and testing process involves the following steps:

1. Data Loading and Preprocessing: Load the dataset, handle missing values, and standardize the features.
2. Train-Test Split: Split the dataset into training and testing sets.
3. Model Training: Train the SVM classifier on the training data.
4. Model Evaluation: Evaluate the model's performance on both the training and testing data using accuracy scores.
## Making Predictions
To make a prediction with new data:

Update the input_data variable in the script with the new data values.  
Run the script to get the prediction result.  
Example:
`input_data = (5, 166, 72, 19, 175, 25.8, 0.587, 51)`
## Results
The model is evaluated using accuracy scores on both the training and testing datasets. The following accuracy scores were achieved:

#### Training Data Accuracy: 
78.66%
#### Test Data Accuracy: 
77.27%  
These results demonstrate the model's ability to predict diabetes with a reasonable degree of accuracy.
## Contributing
Contributions are welcome! If you have any improvements, suggestions, or bug fixes, please create a pull request or open an issue.

1. Fork the repository.
2. Create a new branch (git checkout -b feature-branch).
3. Commit your changes (git commit -am 'Add new feature').
4. Push to the branch (git push origin feature-branch).
5. Create a new Pull Request.
## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Acknowledgements
- The dataset used in this project is provided by the National Institute of Diabetes and Digestive and Kidney Diseases.
- Special thanks to the contributors of the scikit-learn library for providing robust tools for machine learning.
