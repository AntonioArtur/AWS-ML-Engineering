# Smishing Detector
##### Author: Antonio Artur de Holanda e Ayres de Moura
Smishing detector model trained and deployed on SageMaker and served via lambda functions. Detailed information is found in the project report.

## Setup
Use the requirements file to install necessary libraries.
```bash
pip install -r requirements.txt
```

## Dataset
To download the dataset, execute the following commands in order

```bash
wget https://md-datasets-cache-zipfiles-prod.s3.eu-west-1.amazonaws.com/f45bkkt8pr-1.zip
unzip f45bkkt8pr-1.zip
unzip "SMS PHISHING DATASET FOR MACHINE LEARNING AND PATTERN RECOGNITION/Dataset_5971.zip"
```

## Notebooks

##### EDA:
Contains the Exploratory data analysis code.
##### SciKit-Learn
Contains the experiments with scikit-learn models.
##### BERT
Contains the experiments with BERT model.

## Training and deployment

To train and deploy the model simply upload the contents of ./code/SageMaker/training to a notebook instance and execute all cells of "Training Notebook.ipynb".

## Lambda Function

- Create a lambda function using ./code/SageMaker/lambda-function/lambdafunction.py

obs: Change the endpoint name to the one you deployed at the training and deployment step
