# Cybersecurity Threat Classification using Machine Learning

## Project Overview
This project aims to classify cybersecurity threats using machine learning techniques. The dataset used is a network intrusion detection dataset from Kaggle, which contains various network traffic features labeled as normal or attack traffic. The goal is to build predictive models that can effectively detect malicious activity in network data.

## Dataset
- **Source:** [Kaggle Network Intrusion Detection Dataset](https://www.kaggle.com/datasets/sampadab17/network-intrusion-detection)
- The dataset contains a mix of numerical and categorical features representing network traffic characteristics.
- The target column specifies whether the traffic is **normal** or an **attack**.

## Installation & Requirements
Ensure you have the following dependencies installed before running the code:

```sh
pip install pandas numpy scikit-learn seaborn matplotlib tensorflow
```

## Data Preprocessing
The dataset undergoes several preprocessing steps to ensure high-quality input for machine learning models:

1. **Handling Missing Values**  
   - Missing values are either removed or imputed to maintain data consistency.

2. **Encoding Categorical Features**  
   - Categorical variables such as `protocol_type`, `service`, and `flag` are converted into numerical values using **one-hot encoding** or **label encoding**.

3. **Feature Scaling**  
   - Numerical features are standardized using `StandardScaler` from `scikit-learn` to improve model performance.

4. **Splitting Dataset**  
   - The dataset is divided into training and testing sets to evaluate model performance effectively.

---

## Machine Learning Models Used
We implemented multiple machine learning algorithms to classify network threats:

- **Random Forest Classifier**: An ensemble learning method using multiple decision trees.
- **Support Vector Machine (SVM)**: A powerful model effective for high-dimensional data.
- **Logistic Regression**: A simple yet effective classification model.

---

## Model Evaluation
Each model's performance is assessed using the following metrics:

1. **Accuracy Score**  
   - Measures the overall correctness of predictions.

2. **Classification Report**  
   - Includes Precision, Recall, and F1-score for both normal and attack classes.

3. **Confusion Matrix Visualization**  
   - Helps analyze true positive, false positive, true negative, and false negative predictions.

4. **Feature Importance**  
   - For Random Forest, the importance of each feature in decision-making is visualized.

---

## Running the Code
Ensure the dataset is in the same directory as the script, then execute

## Output
Upon execution, the script generates the following outputs:

- **Model Evaluation Metrics**: Accuracy, precision, recall, and F1-score.
- **Confusion Matrices**: Graphical representation of model predictions.
- **Feature Importance Analysis**: Identifies key features influencing predictions.
- **Final Test Predictions**: Saved as `test_predictions.csv`.

## Conclusion
This project demonstrates the effectiveness of machine learning models in classifying cybersecurity threats. By utilizing Random Forest, SVM, and Logistic Regression, we successfully identified patterns in network traffic to distinguish between normal and malicious activity. 

Feature selection and preprocessing played a crucial role in enhancing model performance. The results indicate that machine learning can significantly aid in intrusion detection, but further improvements such as hyperparameter tuning, ensemble learning, and real-time monitoring could enhance accuracy and reliability.

Future work can focus on integrating these models into a live cybersecurity system for proactive threat detection.


