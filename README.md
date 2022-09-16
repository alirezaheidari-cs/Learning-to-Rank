# Implement a pointwise learning to rank algorithm and train on LETOR4.0 dataset

## Prerequisites
- Python 3.6+
- Scikit-learn
- imblearn
- Pyspark


## Accuracy
| Model             | Acc.        |
| ----------------- | ----------- |
| Closed Form Model        | 75.61%      |
| SGDRegressor with oversampling       | 51.93%      |
| SGDRegressor        | 51.93%      |


## EDA
  ### Sparsity
  reduce features dimension due to sparsity using PCA
  
  <h3 align="center">
  <img src="Images/pca.png" width="800">
  </h3>
  change the dimension from 46 to 30 would have no information-loss and speeds up training time.
  
  ### Class Imbalance
  -cope with class imbalance problem with oversampling
  <h3 align="center">
  <img src="Images/imbalance.png" width="800">
  </h3>
  after oversampling, distribution of data separated by labels is shown below:
  <h3 align="center">
  <img src="Images/oversampled.png" width="800">
  </h3>
  
  
