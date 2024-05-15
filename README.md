# Human Activity Recognition

This Jupyter Notebook aims to develop a Human Activity Recognition (HAR) system using machine learning techniques. It involves recording acceleration signals for two activities (**running** and **walking**), loading and visualizing them. After preprocessing for data quality, systematic time-series feature extraction was performed to characterize the signals effectively. These features are then used to create a model to detect the type of motion with high accuracy and practical applicability.

## Installation

This script requires the use of Jupyter Notebook and the following dependencies:
- DateTime (process date/time values)
- Matplotlib (plotting results)
- NumPy (manipulating arrays and apply mathematical operations)
- Pandas (store results and perform)
- Seaborn (statistical data visualisation)
- Scikit-learn (model creation and performance analysis)
- Tsfresh (time-series feature engineering)

```bash
pip install datetime
pip install matplotlib
pip install numpy
pip install pandas
pip install seaborn
pip install scikit-learn
pip install tsfresh
```

## Usage

To use this script, follow these steps:
- Clone the repository or download it as a zip folder and extract all files.
- Ensure you have installed the required dependencies.
- Run the HAR.ipynb notebook and ensure the relative paths to the CSV files are correct.

## Methodology

**Record Acceleration Data**
   - Record linear acceleration data for running and walking activities using the Physics Toolbox Sensor Suite mobile application.
   - Each activity must be at least 2 minutes.
   - Stored as CSV files.

**Loading Data**
   - Load CSV files in for each activity using Pandas.

**Visualise Data**
   - Examine the acceleration signals and determine any obvious differences.
   - Identify transition periods if applicable.

**Preprocess Data**
   - Add additional columns as required and remove redundant information from the signals.

**Feature Extraction**
   - Extract meaningful features from the dataset using Tsfresh.

**Model Creation**
   - Select the best features to explain differences in motion.
   - Build a Random Forest Classifier to detect the type of motion and evaluate its performance.

## Results
Model achieved a mean accuracy of **99.64%** across 10-fold corss-validation. Based on this result, the model's potential for healthcare usage is explored further in the notebook.
