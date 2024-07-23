# Diabetes Prediction

This project predicts whether a person has diabetes using machine learning techniques on the Pima Indians Diabetes Database.

## Table of Contents
- [Installation](#installation)
- [Usage](#usage)
- [Project Structure](#project-structure)
- [License](#license)

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/sattusss/diabetes-prediction.git
   ```
2. Navigate to the project directory:
   ```bash
   cd diabetes-prediction
   ```
3. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

## Usage

To use the prediction system:

1. Load the trained model and scaler.
2. Predict diabetes based on input data:
   ```python
   import numpy as np
   from sklearn.preprocessing import StandardScaler
   from sklearn import svm

   # Example input data
   input_data = (2, 197, 70, 45, 543, 30.5, 0.158, 53)
   input_data_as_numpy_array = np.asarray(input_data)
   input_data_reshaped = input_data_as_numpy_array.reshape(1, -1)
   std_data = scaler.transform(input_data_reshaped)
   prediction = classifier.predict(std_data)

   if (prediction[0] == 0):
       print('The person is not diabetic')
   else:
       print('The person is diabetic')
   ```

## Project Structure

- `Diabetes-Prediction.ipynb`: Jupyter Notebook with the workflow.
- `requirements.txt`: List of dependencies.

## License

This project is licensed under the MIT License.
