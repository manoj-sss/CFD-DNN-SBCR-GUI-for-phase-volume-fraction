# CFD-DNN-SBCR-GUI-for-phase-volume-fraction
This repository provides an integrated solution for predicting and analyzing phase volume fractions in slurry bubble column reactors using deep neural network (DNN) surrogate models trained on CFD simulation data


## File Explanation and Usage Guide

### 1. Jupyter Notebook GUI_DNN_SBCR_CFD.ipynb

This notebook is used for **GUI-based prediction** of CFD results using the trained DNN model.

#### Features

* Upload Excel input files directly for prediction
* Enter operating conditions manually through the GUI
* Predict output values using the trained model

#### Required Files

To run this notebook successfully, keep the following files in the same folder:

* Cfd_weights.weights.h5
* scaler.save
* Sample Excel file: ug.xlsx

#### Purpose

This notebook is suitable for users who want an easy graphical interface for predictions without modifying the code.

---

### 2. Jupyter Notebook DNN_SBCR_Phase_Volume Fraction.ipynb

This notebook is used for prediction with a **single combination of operating conditions** or an **Excel file of input parameters**.

#### Features

* Predict values for manually entered operating conditions
* Test individual input combinations
* Run direct model predictions without GUI interaction

### 3. Cfd_weights.weights.h5

This file contains the **trained weights of the Deep Neural Network (DNN) model**.

#### Purpose

* Stores the learned parameters of the trained model
* Required during prediction
* Loaded automatically by the notebooks


### 4. scaler.save

This file contains the **saved scaler object** used during model training.

#### Purpose

* Scales and normalizes the input data before prediction
* Ensures prediction accuracy by using the same preprocessing applied during training

> This file is required to run predictions correctly.

### 5. Sample Excel File: ug.xlsx

This is a sample input Excel file provided for testing the GUI prediction notebook.

#### Purpose

* Demonstrates the required input format
* Helps users understand how to prepare input data
* Can be uploaded directly in the GUI notebook

## How to Run the Project

1. Place all files in the same directory/folder.
2. Open the required notebook using Jupyter Notebook or JupyterLab.
3. Run all cells sequentially.
4. For GUI prediction:

   * Open GUI_DNN_SBCR_CFD.ipynb
   * Upload ug.xlsx or enter values manually
5. For direct prediction:

   * Open DNN_SBCR_Phase_Volume Fraction.ipynb
   * Enter operating conditions in the input section
6. Ensure both:

   * Cfd_weights.weights.h5
   * scaler.save`

  are available in the same folder before running the notebooks.


