# Efficient Intrusion Detection System for IoT Environments using Feature Selection and Ensemble Soft Voting Classifier
# Overview
The rapid growth of the Internet of Things (IoT) has introduced new security challenges due to the limited security capabilities of many IoT devices. Traditional Intrusion Detection Systems (IDS) often struggle to handle the large-scale, dynamic, and heterogeneous nature of IoT networks.
This project presents a Machine Learning–based Intrusion Detection System (IDS) designed specifically for IoT environments. The system improves intrusion detection performance by applying feature selection techniques and an ensemble soft voting classifier. The proposed model combines multiple machine learning algorithms to improve detection accuracy and reliability when identifying malicious network activities.
This project was developed as part of an undergraduate research project in the Department of Computer Science, Federal University, Kashere, Gombe state, Nigeria.

# Dataset
The model was trained and evaluated using the NSL-KDD dataset, a widely used dataset for intrusion detection research.
Dataset details:
| Dataset      | Instances | Features |
| ------------ | --------- | -------- |
| Training Set | 125,973   | 41       |
| Testing Set  | 22,544    | 41       |

During preprocessing, the dataset was converted from multiclass classification to binary classification, categorizing network traffic as:
- Normal
- Abnormal (Attack)

# Methodology
The proposed system follows the following pipeline:
1. Data Collection and Preprocessing
  - NSL-KDD dataset preparation
  - Data cleaning and transformation
  - Conversion of multiclass labels to binary classes

2. Feature Selection
Two filter-based feature selection techniques were used:
  - Chi-Square
  - Mutual Information

These techniques help reduce dimensionality by selecting the most relevant features for classification.

3. Model Development
An ensemble soft voting classifier was developed using three machine learning algorithms:
  - Random Forest (RF)
  - Logistic Regression (LR)
  - Artificial Neural Network (ANN)
The final prediction is obtained by combining the probabilities of all classifiers.

4. Model Evaluation
The model performance was evaluated using standard classification metrics.

# Results
The proposed IDS achieved the following performance:
| Metric    | Value      |
| --------- | ---------- |
| Accuracy  | **99.40%** |
| Precision | **99.12%** |
| Recall    | **99.76%** |
| F1 Score  | **99.44%** |

# Technologies Used
- Python
- Scikit-learn
- Pandas
- NumPy
- Matplotlib / Seaborn
- Machine Learning Algorithms


