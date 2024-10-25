# Smart Irrigation System with Machine Learning on Raspberry Pi

## Abstract
Conventional farming has been a cornerstone of human existence, with water being a critical resource for both agriculture and the general population. The growing demand for sustainable irrigation methods has led to the development of smart systems that integrate Artificial Intelligence (AI) and IoT. This project presents a cost-effective and resource-efficient irrigation method built on Raspberry Pi, using various sensors and machine learning to optimize water usage.

## Introduction
Water resource management is crucial for sustainable agriculture, especially in the face of rising demands and limited supplies. Traditional irrigation systems rely on fixed schedules, which may lead to inefficiencies. This project aims to create a smart irrigation system that adapts to environmental changes and optimizes water usage using IoT sensors and machine learning.

## Related Work
The integration of AI in agriculture, known as AI4AI (Artificial Intelligence for Agricultural Innovation), has been gaining traction. This approach enables better yield management and resource optimization. Notable implementations include Microsoft’s work with farmers in Andhra Pradesh, India, which led to a 30% increase in crop yield. Several machine learning models, such as SVM, Naive Bayes, and Neural Networks, were explored for this project to achieve high accuracy and adaptability.

## Data
The dataset includes readings from humidity and temperature sensors and binary pump values indicating when plants need water. The collected data represents various crops with different water requirements. Soil humidity and temperature were recorded using analog sensors, with average readings of 384.5 for soil humidity and 26.34°C for temperature.

## Methods
The machine learning models applied include:
- **K-Nearest Neighbors (KNN)**: Classifies data points based on nearest neighbors, achieving 76% accuracy.
- **Support Vector Machine (SVM)**: Separates data using a hyperplane, achieving 76% accuracy.
- **Random Forest**: An ensemble method that builds multiple decision trees, with 69% accuracy.
- **AdaBoost**: Combines weak learners to improve accuracy, achieving 77% accuracy, making it the most effective model in this project.
  
After training, the best model, AdaBoost, was converted to TensorFlow Lite format and deployed on Raspberry Pi.

## Experiments
Different models were tested to compare their performance on the dataset:
- KNN, Gradient Boosting Classifier, and SVM performed well with moderate accuracy.
- XGBoost and Random Forest encountered reduced accuracy with larger datasets.
- AdaBoost provided the highest accuracy at 77%, making it the preferred model for deployment.

## Conclusion
This project demonstrates a smart irrigation system that uses sensors and machine learning to optimize water use in agriculture. The AdaBoost model, deployed on a Raspberry Pi, showed a superior accuracy rate and adaptability. Future improvements include optimizing sensor quality for more efficient water management.

## Implementation
The smart irrigation model was implemented on a Raspberry Pi using Node-RED. Sensor data was imported through Raspberry Pi's command prompt and deployed on Node-RED for real-time monitoring.

---

**Keywords**: Machine Learning, Raspberry Pi, IoT, Irrigation, AdaBoost, Agriculture 4.0
