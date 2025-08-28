# Intent Classification for Banking Customer Queries

This project compares traditional machine learning models (Logistic Regression, SVM) with a deep learning model (BiLSTM) for intent classification on the BANKING77 dataset. The goal is to classify customer service queries into 77 predefined banking intents.

## 📊 Dataset
- **BANKING77**: Contains 13,083 English customer service queries labeled into 77 fine-grained intents.
- Source: [PolyAI GitHub Repository](https://github.com/PolyAI-LDN/task-specific-datasets)
- License: CC-BY-4.0

## 🧠 Models Implemented
1. **Logistic Regression** (with TF-IDF + word/char n-grams)
2. **Support Vector Machine (SVM)** (with TF-IDF + word/char n-grams)
3. **Bidirectional LSTM (BiLSTM)** (with word/char embeddings)

## 📈 Results
| Model       | Accuracy | Macro F1 | Training Time | Model Size |
|-------------|----------|----------|---------------|------------|
| Logistic Regression | 0.8886 | 0.8888   | 32.004s       | 23.7MB     |
| SVM         | 0.9029   | 0.9030   | 6.494s        | 10.1MB     |
| BiLSTM      | 0.8860   | 0.8863   | 2411.88s      | 45.6MB     |

## 🚀 Usage
### Prerequisites
- Python 3.7+
- Install dependencies:  
  ```bash
  pip install -r requirements.txt
