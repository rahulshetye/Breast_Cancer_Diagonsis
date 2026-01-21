# Breast_Cancer_Diagonsis

Objective: Build a supervised machine learning model to classify a tumor as Malignant (M) or Benign (B) and demonstrate the complete ML workflow (problem framing → data prep → model training → evaluation → error analysis). 
Dataset (link): 
https://archive.ics.uci.edu/dataset/17/breast+cancer+wisconsin+diagnostic  
Expected Input (for your program/submission): 
data.csv (downloaded from the dataset link; features + target label) 
A command-line interface like: 
python task1_cancer_classification.py --data data.csv --test_size 0.2 --model logistic 
Expected Output: 
Train error and Test error (report both; show generalization gap) 
Accuracy, Precision, Recall, F1-score on test set 
Confusion matrix (as printed matrix/table) 
A short conclusion: whether model shows overfitting/underfitting and why (1–2 paragraphs) 
Minimum tasks to perform: 
Split into train/test (or train/val/test) 
Standardize/normalize features where applicable 
Train Logistic Regression (baseline) and Decision Tree (non-linear model) 
Compare: 
training vs test performance 
identify overfitting signs (high train, lower test) 
