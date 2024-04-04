# Challenge 13
## Venture Funding with Deep Learning

## Overview
In this project, we aim to create a binary classifier model using deep learning techniques to predict the success of startup applicants funded by Alphabet Soup, a venture capital firm. The dataset contains information about various organizations that received funding from Alphabet Soup, including features that might influence their success.

## Project Structure
The project is divided into several key steps:

1. **Data Preparation:**
   - Read the `applicants_data.csv` file into a Pandas DataFrame.
   - Drop irrelevant columns such as "EIN" and "NAME".
   - Encode categorical variables using OneHotEncoder.
   - Combine encoded variables with numerical variables.
   - Split the data into features (`X`) and target (`y`) datasets.
   - Split the data into training and testing datasets.
   - Scale the features data using StandardScaler.

2. **Model Compilation and Evaluation:**
   - Create a deep neural network model using TensorFlow's Keras.
   - Compile the model with binary_crossentropy loss function, adam optimizer, and accuracy metric.
   - Fit the model to the training data.
   - Evaluate the model's performance using the test data.

3. **Model Optimization:**
   - Define alternative deep neural network models to improve predictive accuracy.
   - Experiment with adjusting input data, adding more neurons or layers, using different activation functions, or changing the number of epochs.
   - Evaluate the performance of each alternative model and compare the results.
   - Save each optimized model as an HDF5 file.

## Files included
- **`AlphabetSoup.h5`:** HDF5 file containing the optimized parameters of the original model.
- **`AlphabetSoup_A1.h5`:** HDF5 file containing the optimized parameters of the first alternative model.
- **`AlphabetSoup_A2.h5`:** HDF5 file containing the optimized parameters of the second alternative model.
- **`README.md`:** This file, providing an overview of the project, its structure, and key steps.


## Dependencies
- pandas
- scikit-learn
- TensorFlow
- Keras
