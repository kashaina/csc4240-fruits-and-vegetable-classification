# Setting up the Environment for Classifiers

This guide shows you how to run the SVM and NN with the provided HDF5 files
**NOTE: These instructions have worked on some machines but not on other machines. The problem is yet undetermined.**

## Instructions to Run the Model

### Step 1: Installation
1. Install **Visual Studio Code (VSCode)** if not already installed
2. Open VSCode and download the **Jupyter** extension from the Visual Studio Code Marketplace

### Step 2: Project Setup
1. Open the project folder in VSCode and set it as the working directory
2. Ensure the working directory contains the following files:
- `classifiers.ipynb`
- `preprocessing_requirements.txt`
- `preprocessing.ipynb`
- `README.md`
- `requirements.txt`
- `validation_fruits_NEWEST_dataset.h5`
- `test_fruits_NEWEST_dataset.h5`
- `train_fruits_NEWEST_dataset.h5`

### Step 3: Python and Depencies Installation
1. Ensure you have **Python 3.11.6** downloaded and installed on your system, or download here: **https://www.python.org/downloads/release/python-3116/**
2. Open a terminal within VSCode, set this directory as the working directory, and run the following command:
```bash
pip install -r requirements.txt
```

### Step 4: Models Exectuion
1. Open **models.ipynb** in VSCode
2. Do **(Windows) CTRL + Shift + P** or **(Mac) CMD + Shift + P** and select **Python: Select Interpreter**
3. Select **Python 3.11.6**
3. Execute the cells in models.ipynb from top to bottom
4. Watch the models run!






## Instructions to Transform the Data (**NOT REQUIRED!**)

**Because the images are already cleaned, augmented, and provided as HDF5 files in this folder, these steps are not necessary.**
However, if you wish to run these instructions with the complete, unclean dataset, follow these instructions below in addition to the steps above

### Step 1: Data Collection
1. Download the dataset found here: **https://www.kaggle.com/datasets/kritikseth/fruit-and-vegetable-image-recognition/data?select=test**

### Step 2: Dependency Installation
1. Open a terminal within VSCode, set this directory as the working directory, and run the following commandz\s:
```bash
pip install -r preprocessing_requirements.txt
pip install hashlib
pip install os-sys
```

### Step 3: Code Setup
**NOTE: As specified in preprocessing.ipynb, you will have to run this code three times with train, test, and validate**
1. Open **preprocessing.ipynb** in VSCode
2. Change the line in cell 1 with your chosen set of images, such as train: ``directory = 'Path\\To\\train_or_validate_or_test'``
3. Change the line in cell 2 to your directory with the chosen set of images: ``directory = 'C:\\Users\\vange\\OneDrive - Tennessee Tech University\\Desktop\\Fall 23\\4240\\proj\\validation'``
4. Change the line in cell 3 with the chosen set of images: ``directory = 'Path\\To\\train_or_validate_or_test'``
5. Change the line in cell 4 with your fruits directory: ``directory = 'Path\\To\\fruits_directory'``
6. Repeat steps 2-5 with your other data sets

### Step 4: Code Execution
1. Do **(Windows) CTRL + Shift + P** or **(Mac) CMD + Shift + P** and select **Python: Select Interpreter**
2. Select **Python 3.11.6**
3. Execute the cells in models.ipynb from top to bottom
4. Watch the code run!