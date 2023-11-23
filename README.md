# Kidney-Tumor-Classification-MLFLOW
This project is the complete workflow of providing and maintaining the life cycle of a model using MLflow to classify image contain Tumor in CT-Scan's images with deployment of the model.

## Workflows

1. Update config.yaml
2. Update params.yaml
3. Update the entity
4. Update the configuration manager in src config
5. Update the components
    - data ination
    - model training
    - model evaluation
    - etc.
6. Update the pipeline 
    - pipline for training an prediction
7. Update the main.py --> Our Endpoints
8. Update the dvc.yaml
9. app.py --> Flask app


# How to run?
### STEPS:

Clone the repository

```bash
git clone https://github.com/parham075/Kidney-Tumor-Classification.git
```
### STEP 01- Create a mamba environment after opening the repository

```bash
mamba create -n kidney python=3.8 -y
```

```bash
mamba activate kidney
```

### STEP 02- install the requirements
```bash
pip install -r requirements.txt
```

```bash
# Finally run the following command
python app.py
```

Now,
```bash
open up you local host and port
```


### dagshub
Connect to the remote repository using Dagshub from [dagshub](https://dagshub.com/)

> MLFLOW_TRACKING_URI=<dagsub_uri_in_experiments>/
MLFLOW_TRACKING_USERNAME=Parham075 (github_user_name) \
MLFLOW_TRACKING_PASSWORD=<dagshub_pass_in_experiments> \
python script.py

Run this to export as env variables:

```bash

export MLFLOW_TRACKING_URI=<dagsub_uri_in_experiments>

export MLFLOW_TRACKING_USERNAME=Parham075 

export MLFLOW_TRACKING_PASSWORD=<dagshub_pass_in_experiments>

```