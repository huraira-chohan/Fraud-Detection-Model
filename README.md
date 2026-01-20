Overview

This project focuses on detecting fraudulent transactions using LightGBM , a grading boosting model. The fraud data is highly imbalanced, so the model is designed to catch as many fraud cases as possible while keeping false alerts reasonable.

The model achieves high recall on the minority class (fraud) and a ROC-AUC of around 0.92, showing strong ability to distinguish fraud from normal transactions.

Features

Uses LightGBM for fast and accurate gradient boosting.

Handles extremely imbalanced datasets effectively.

Optimized for high recall, ensuring most fraud cases are detected.

Supports custom thresholding to balance recall vs precision.

Includes stratified train/test splitting to maintain class proportions.

Performance

The model’s performance on test data is strong:

ROC-AUC: 0.918

Recall (fraud detection): 0.88

Precision: ~0.035

Note: Precision is low due to the rarity of fraud cases, but the main priority is catching fraud rather than avoiding false positives.

How It Works

Prepare the dataset with features and labels.

Split the data into training and test sets, preserving class distribution.

Train LightGBM with tuned parameters to handle imbalance and weak signals.

Evaluate the model using metrics that matter for fraud detection, like recall and ROC-AUC.

Why This Matters

Fraud detection is a critical real-world problem, and models like this can help reduce financial losses while prioritizing risky transactions for review. By focusing on recall and using gradient boosting, this approach is both practical and powerful for real-world applications.
