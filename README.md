{
 "cells": [
  {
   "cell_type": "markdown",
   "id": "877094f8-b99b-411a-b3bf-bedb1122c205",
   "metadata": {},
   "source": [
    "# Cybersecurity Threat Classification using Machine Learning\n",
    "\n",
    "## Project Overview\n",
    "\n",
    "This project focuses on classifying cybersecurity threats using machine learning techniques. The dataset used is a network intrusion detection dataset from Kaggle, and the goal is to build models that can accurately distinguish between normal and attack traffic.\n",
    "\n",
    "## Dataset\n",
    "\n",
    "- Source: [Kaggle Network Intrusion Detection Dataset](https://www.kaggle.com/datasets/sampadab17/network-intrusion-detection)\n",
    "- The dataset consists of various network traffic features and a target column indicating whether the traffic is normal or an attack.\n",
    "\n",
    "## Data Preprocessing\n",
    "- Handling missing values\n",
    "- Encoding categorical features (protocol_type, service, flag)\n",
    "- Feature scaling using StandardScaler\n",
    "- Splitting dataset into train and test sets\n",
    "\n",
    "## Machine Learning Models Used\n",
    "- Random Forest Classifier\n",
    "- Support Vector Machine (SVM)\n",
    "- Neural Network (MLPClassifier)\n",
    "- XGBoost Classifier (if installed)\n",
    "\n",
    "## Model Evaluation\n",
    "- Accuracy Score\n",
    "- Classification Report\n",
    "  \n",
    "  ![Image](report.png)\n",
    "  \n",
    "- Confusion Matrix Visualization\n",
    "- Feature Importance (for Random Forest)\n",
    "  \n",
    "  ![Image](perf.png)\n",
    "\n",
    "## Output\n",
    "- Model evaluation metrics\n",
    "- Confusion matrices for each model\n",
    "- Feature importance visualization\n",
    "- Final test predictions saved as test_predictions.csv"
   ]
  }
 ],
 "metadata": {
  "kernelspec": {
   "display_name": "Python 3 (ipykernel)",
   "language": "python",
   "name": "python3"
  },
  "language_info": {
   "codemirror_mode": {
    "name": "ipython",
    "version": 3
   },
   "file_extension": ".py",
   "mimetype": "text/x-python",
   "name": "python",
   "nbconvert_exporter": "python",
   "pygments_lexer": "ipython3",
   "version": "3.12.7"
  }
 },
 "nbformat": 4,
 "nbformat_minor": 5
}
