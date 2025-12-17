Customer Churn Classification using ANN
This project implements an Artificial Neural Network (ANN) to predict customer churn for a bank. The goal is to identify customers who are likely to leave the bank based on various demographic and financial factors, allowing the bank to take proactive measures to retain them.

📌 Project Overview
Customer churn happens when customers stop doing business with a company. In the banking sector, it is much cheaper to retain existing customers than to acquire new ones. This project uses deep learning to classify customers into two categories:
0: Customer stays with the bank.
1: Customer exits the bank.
📊 Dataset
The project typically uses the Churn_Modelling.csv dataset, which includes the following features:
Geography: Country of the customer.
Gender: Male or Female.
Credit Score: Numerical value representing creditworthiness.
Age: Age of the customer.
Tenure: Number of years the customer has been with the bank.
Balance: Account balance.
NumOfProducts: Number of bank products the customer uses.
HasCrCard: Whether the customer has a credit card.
IsActiveMember: Whether the customer is an active member.
EstimatedSalary: Annual salary of the customer.
Exited: (Target Variable) Whether the customer left the bank.

🛠️ Tech Stack
Language: Python
Libraries: - Pandas & NumPy: For data manipulation.
Scikit-learn: For data preprocessing (Label Encoding, One-Hot Encoding, Feature Scaling).
TensorFlow / Keras: For building and training the Artificial Neural Network.
Matplotlib / Seaborn: For data visualization.

🚀 Key Steps in the Project
1. Data Preprocessing
Handled categorical data using Label Encoding (for Gender) and One-Hot Encoding (for Geography).
Split the data into Training and Testing sets.
Applied Feature Scaling (StandardScaler) to normalize the input data, which is crucial for the convergence of an ANN.
2. Building the ANN
Input Layer: Based on the number of features.
Hidden Layers: Multiple dense layers with ReLU activation function.
Output Layer: A single neuron with a Sigmoid activation function (for binary classification).
3. Training the Model
Optimizer: Adam
Loss Function: binary_crossentropy
Metrics: accuracy
Epochs: Trained over multiple iterations to minimize loss.
4. Evaluation
Prediction on test data.
Generation of a Confusion Matrix.
Calculation of the Accuracy Score.
💻 How to Run
Clone the repository:
Bash
git clone https://github.com/himanshu9325/ANN_Chrun_Clasification.git
Navigate to the folder:
Bash
cd ANN_Chrun_Clasification
Install dependencies:
Bash
pip install tensorflow pandas scikit-learn numpy
Run the script or Jupyter Notebook:
Bash
python churn_classification.py
📈 Results
The model achieves a high accuracy rate (typically around 83-86%) in predicting customer behavior, providing valuable insights into the primary drivers of customer churn.

🤝 Contributing
Contributions, issues, and feature requests are welcome! Feel free to check the issues page.

📝 License
This project is MIT licensed.
