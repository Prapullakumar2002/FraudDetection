# FraudDetection

# 🛡️ Real-Time Credit Card Fraud Detection using Random Forest

This project demonstrates a complete fraud detection pipeline using a Random Forest Classifier, applied on a transaction dataset. It simulates **real-time fraud detection** by processing transaction samples and printing alerts when fraud is detected.


## 📂 Dataset

The dataset is assumed to be a cleaned version of `transactionsSmall.csv`, containing anonymized transaction records. It includes features such as:
- `step`, `type`, `amount`
- `oldbalanceOrg`, `newbalanceOrig`, `oldbalanceDest`, `newbalanceDest`
- `isFraud` (target variable)

---

## 🧠 Model

We use the **Random Forest Classifier**, which works well for tabular data like financial transactions. It achieves high accuracy and detects frauds with precision.

---

## 📦 Project Structure
fraud-detection/
│
├── transactionsSmall.csv # Input dataset
├── fraud_detection.py # Main script
├── README.md # Project documentation
└── requirements.txt # Python dependencies


## ⚙️ Steps Covered

1. **Data Loading & Exploration**  
   Read the dataset and check for missing values.

2. **Preprocessing**  
   - Encode the `type` categorical feature.
   - Scale the numerical features using `StandardScaler`.

3. **Train-Test Split**  
   Train the model on 80% data and evaluate on 20%.

4. **Model Training**  
   Train a `RandomForestClassifier` and print accuracy & classification report.

5. **Real-Time Simulation**  
   Pick 100 random transactions from the test set and simulate fraud detection.

---

🚀 How to Run

1. Clone the repository

```bash
git clone https://github.com/your-username/fraud-detection.git
cd fraud-detection

2. Install dependencies
pip install -r requirements.txt

3. Add your dataset
Place transactionsSmall.csv in the root directory. Adjust the path if necessary in the code.

4. Run the main script
python fraud_detection.py

You’ll see real-time output like:
✅ Transaction ID 101 is Safe.
🚨 Fraud Detected in Transaction ID 172

🧪 Sample Output
Model Accuracy: 99.37%

               precision    recall  f1-score   support
           0       0.99      1.00      1.00       409
           1       1.00      0.96      0.98        68
📋 Dependencies
Add the following to your requirements.txt:
pandas
numpy
scikit-learn

👨‍💻 Author
K.prapulla kumar

https://github.com/Prapullakumar2002




