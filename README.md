# Analyzing the effectiveness of synthetic data on learning models which train on scarce datasets

Levi Pare, Rivier Bunpas, Jack D'Iorio

Goal: Best accuracy for public model which satisfies DP and utilizes sensitive data which is scarce

Problem: 
- Sensitive dateset has few entries
- Want a publicly available learning model which given sensitive scarce data can predict label

Note: we are using public data for ease of collection, show how this could apply to real world scenarios

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
