# Assessing Model Performance: Synthetic Data and Differential Privacy for Scarce Sensitive Datasets

Levi Pare, River Bumpas, Jack D'Iorio

Goal: Best accuracy for public model which satisfies DP and utilizes sensitive data which is scarce

Problem: 
- Sensitive dateset has few entries
- Want a publicly available learning model which given sensitive scarce data can predict label

Note: we are using public data for ease of collection, show how this could apply to real world scenarios

(Open to change, please modify if necessary)
Hypothesis: Training a classification model on synthetic data generated from the original dataset yields a more accurate model than one trained on the original dataset where the output of either system satisfies epsilon-delta Differential Privacy.

**ADDRESS THE FACT THAT synth-noise USES APPROXIMATE DIFF. PRIV. AND dp_decisiontree USES PURE EPSILON DIFF. PRIV**

## Todo
- [x] Submit proposal
- [x] Submit CS Fair
- [ ] Generate graphical model
- [ ] Sythetic data by 2-way marginals
- [ ] ML model architecture
      - Model?
      - Loss function?
      - Activation function?
- [ ] Stochastic Gradient Descent

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


## Notes:
- We want a Multi-layer Perception (MLP) for this classification problem
- Must do best to ensure quality of synthetic data or it will affect downstream results
- Must have a maximum epsilon value which methods can meet but must not exceed, less epsilon is okay for more accuracy (CHECK THIS POINT)
- Must use same data split (train / test) for methods 1,2 and 3,4
