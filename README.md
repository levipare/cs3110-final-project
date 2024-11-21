# Assessing Model Performance: Synthetic Data and Differential Privacy for Scarce Sensitive Datasets

Levi Pare, River Bumpas, Jack D'Iorio

Goal: Best accuracy for public model which satisfies DP and utilizes sensitive data which is scarce

Problem: 
- Sensitive dateset has few entries
- Want a publicly available learning model which given sensitive scarce data can predict label

Note: we are using public data for ease of collection, show how this could apply to real world scenarios

(Open to change, please modify if necessary)
Hypothesis: Training a classification model on synthetic data generated from the original dataset yields a more accurate model than one trained on the original dataset where the output of either system satisfies epsilon-delta Differential Privacy.

## Tests

### Method 1:
Generate synthetic data with noise and then train public model on that

### Method 2:
Generate synthetic data without noise and train DP public model

## Baselines:

### Method 3:
Train DP public model on original low count data

### Method 4:
Train public model on noisy original data


## Notes:
- We want a Multi-layer Perception (MLP) for this classification problem
