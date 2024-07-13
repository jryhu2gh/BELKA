# BELKA
Based on Kaggle competetion Belka. Self implemented. Needs to be improved
Transformer based model. Binary classification. Imbalanced data training.

# Training Data
This competetion has an imbalanced data. The number of possitive class is much less than negative class. Besides, the training data is extremely large, difficult to be loaded on a customer-level GPU (4060, 8GB). Two methods are employed to overcome this challenge.
  1. Separate the entire dataset into multiple pages and train them in turn
  2. Downsample the ratio of negative class in training dataset. All positive data is used, while negative data is randomly sampled with a specified ratio.

To be studied: use ROC curve to study how to balance the interpretion of the prediction
