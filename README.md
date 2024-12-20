# Assessing Model Performance: Synthetic Data and Differential Privacy for Scarce Sensitive Datasets

Levi Pare, River Bumpas, Jack D'Iorio

Goal: Best accuracy for public model which satisfies DP and utilizes sensitive data which is scarce

Problem: 
- Sensitive dateset has few entries
- Want a publicly available learning model which given sensitive scarce data can predict label

Note: we are using public data for ease of collection, show how this could apply to real world scenarios

(Open to change, please modify if necessary)
Hypothesis: Training a classification model on synthetic data generated from the original dataset yields a more accurate model than one trained on the original dataset where the output of either system satisfies epsilon-delta Differential Privacy.


## Setup
Run the following commands in the project directory to setup the enviroment.

```
python3 -m venv .venv
source .venv/bin/activate
pip install ipykernel
python -m ipykernel install --user --name=.venv
pip install -r requirements.txt
```

Make sure to select venv as the kernel in jupyter notebook.

## Tests

### Method 1:
Generate synthetic data with noise and then train public model on that

### Method 2:
Generate synthetic data without noise and train DP public model

## Baselines:

### Method 3:
Train DP public model on original low count data

### Method 4:
Train public model on original data
