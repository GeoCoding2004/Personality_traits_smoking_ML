# Cigarette Consumption Prediction Based on Personality Traits
This project explores the relationship between personality traits and smoking behaviors. The primary objective is to predict the number of cigarettes an individual smokes per day (in categorized ranges) based on their psychological attributes and related factors. The study leverages two predictive modeling approaches to address this problem: multinomial logistic regression and fully connected neural networks.

## Dataset
The dataset includes personality trait responses and smoking behavior data. Personality traits are mapped to numerical values, and the target variable represents categorized ranges of daily cigarette consumption:
0–10 cigarettes/day
11–20 cigarettes/day
21–30 cigarettes/day
31+ cigarettes/day

## Methods
### Multinomial Logistic Regression (Softmax model):
A straightforward classification model is used as a baseline.
Accuracy: 53.65%
Observations: Lower accuracy due to class imbalance, especially for higher cigarette consumption categories.


### Fully Connected Neural Network:
Addresses class imbalance using data augmentation for underrepresented categories.
Incorporates a multi-layer perceptron with ReLU activation and softmax for output.
Accuracy: 82.46%
Observations: The model effectively captures non-linear relationships and improves predictive accuracy by handling augmented and balanced data.
Key Features
Class Imbalance Handling:
Data augmentation was applied to increase the sample size of underrepresented classes (21–30 and 31+ cigarettes/day).
Comparative Analysis:
Logistic regression and neural network approaches are compared to demonstrate the effectiveness of more advanced models for complex datasets.
Confusion Matrix Visualization:
Confusion matrices are used to evaluate classification performance for both methods.
Results
Logistic regression is a simpler approach but struggles with imbalanced data, achieving an accuracy of 53.65%.
The neural network, coupled with data augmentation, significantly outperforms logistic regression, achieving an accuracy of 82.46%.
These results highlight the importance of addressing class imbalance and selecting appropriate modeling techniques.
Conclusion
The findings demonstrate that personality traits are significant predictors of smoking behavior. The project underscores the importance of addressing class imbalance and highlights the advantages of neural networks in capturing complex relationships in data.

Contents
Data Preprocessing: Data mapping, handling missing values, and scaling.
Model Training and Evaluation: Implementation of logistic regression and neural networks.
Performance Comparison: Detailed analysis of both approaches.
Confusion Matrix Visualization: Evaluation of class-wise performance.
Future Directions
Explore additional features or data sources to improve predictions further.
Investigate other machine learning models like ensemble methods (e.g., random forests, XGBoost).
Apply explainability techniques to interpret the influence of specific personality traits on smoking behavior.
This notebook serves as a comprehensive guide for exploring the impact of personality traits on smoking behavior and demonstrates the application of machine learning techniques to tackle real-world predictive tasks.
