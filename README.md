# 💳 Online Payment Fraud Detection

This project implements a **machine learning-based fraud detection system** for online payment transactions.  
It analyzes transaction data to identify potentially fraudulent activities, helping financial institutions and e-commerce platforms reduce losses.

## 📌 Features
- Data preprocessing and cleaning
- Exploratory Data Analysis (EDA) with visualizations
- Feature engineering for fraud detection
- Model training with classification algorithms
- Model evaluation using accuracy, precision, recall, F1-score, and confusion matrix
- Fraud probability predictions for new transactions

## 📂 Project Structure

online-payment-fraud-detection/
│
├── data/                     # Raw and processed datasets
│   └── transactions.csv
│
├── notebooks/                # Jupyter Notebooks
│   └── Online payment fraud detection.ipynb
│
├── src/                      # Python scripts for data processing & modeling
│   ├── data_preprocessing.py
│   ├── eda.py
│   ├── model_training.py
│   └── model_evaluation.py
│
├── requirements.txt          # Python dependencies
├── README.md                 # Project documentation



## 🛠️ Technologies Used
- **Python** 3.x
- **Pandas** – Data manipulation
- **NumPy** – Numerical computing
- **Matplotlib / Seaborn** – Data visualization
- **Scikit-learn** – Machine learning algorithms & evaluation metrics

## 📊 Dataset
The project uses a transactional dataset containing fields like:
- `step` – Time step (hours since start)
- `type` – Transaction type
- `amount` – Amount transferred
- `nameOrig` / `nameDest` – Sender and receiver IDs
- `oldbalanceOrg` / `newbalanceOrig` – Sender balance before/after transaction
- `oldbalanceDest` / `newbalanceDest` – Receiver balance before/after transaction
- `isFraud` – Fraud label (1 = Fraud, 0 = Genuine)

**Note:** The dataset used here is for educational purposes and may be synthetic.

## 🚀 How to Run
1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/online-payment-fraud-detection.git
   cd online-payment-fraud-detection
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
3. Run in jupyter notebook:
   ```bash
   jupyter notebook "Online payment fraud detection.ipynb"
4. Run as Python scripts (optional):
If you want to execute the workflow without the notebook:
   ```bash
   python src/data_preprocessing.py
   python src/model_training.py
   python src/model_evaluation.py
5. Run all cells to train the model and view results.

## 📈 Model Performance
The notebook evaluates multiple classifiers and selects the best-performing one based on fraud detection metrics such as:
* Accuracy
* Precision
* Recall
* F1-score

## 🔮 Future Improvements
* Deploy as a web API for real-time fraud detection
* Integrate deep learning models for improved accuracy
* Add streaming data processing with Apache Kafka or Spark


