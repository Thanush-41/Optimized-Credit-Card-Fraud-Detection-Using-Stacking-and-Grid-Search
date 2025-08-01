# Optimized Credit Card Fraud Detection Using Stacking and Grid Search Techniques

##  Overview

This project presents a robust machine learning solution for **credit card fraud detection** using a hybrid model that combines **stacking ensemble learning** and **grid search optimization**. The proposed **GridStack** architecture significantly enhances fraud detection performance by integrating multiple base models and fine-tuning hyperparameters to achieve **98% accuracy**.

##  Highlights

- Ensemble-based hybrid model with **stacking**
- Parameter tuning using **grid search**
- Achieved **98% accuracy**, **96% precision**, **96% recall**, and **96% F1-score**
- Compared against models like Random Forest, Isolation Forest, LSTM, Autoencoders, GCN, SVM, and KNN
- Built and validated on a **balanced Kaggle credit card transaction dataset**



##  Dataset

- Source: [Kaggle - Credit Card Fraud Detection](https://www.kaggle.com/mlg-ulb/creditcardfraud)
- Size: 284,807 transactions
- Balanced for both fraudulent and non-fraudulent cases using PCA anonymization

## ⚙️ Methodology

###  1. Stacking Ensemble

Multiple classifiers are trained individually and combined using a meta-classifier to improve predictive performance:
- Base Models: Random Forest, Isolation Forest, LSTM, Autoencoder, SVM, KNN
- Meta-Model: Logistic Regression or another classifier
- Output: Combines base predictions for final fraud classification

###  2. Grid Search Optimization

- All model hyperparameters are tuned using exhaustive **Grid Search**
- Evaluated using metrics like **F1-score**, **ROC-AUC**, and **Precision-Recall**

## 📈 Results

| Model             | Accuracy | Precision | Recall | F1-Score |
|------------------|----------|-----------|--------|----------|
| Autoencoder       | 92%      | 90%       | 88%    | 89%      |
| LSTM              | 96%      | 94%       | 92%    | 93%      |
| Random Forest     | 95%      | 93%       | 91%    | 92%      |
| Isolation Forest  | 93%      | 91%       | 89%    | 90%      |
| GCN               | 94%      | 92%       | 90%    | 91%      |
| KNN               | 91%      | 89%       | 87%    | 88%      |
| SVM               | 92%      | 90%       | 88%    | 89%      |
| **GridStack**     | **98%**  | **96%**   | **96%**| **96%**  |

##  Evaluation Metrics

- **Confusion Matrix**
- **ROC-AUC Curve**
- **Precision-Recall Curve**
- **F1 Score**



## 📚 Future Work

- Integration with **transformer-based models**
- **Online learning** and **reinforcement learning** for evolving fraud patterns
- Adding **XAI** (Explainable AI) for better interpretability
- Deployment as a **real-time microservice**

## 👨‍💻 Authors

- Siddique Ibrahim S. P
- Lohitha Koneru
- Thanush Chowdary Garimella
- Abhinay Mitta

## 📄 License

This project is open source and available under the [MIT License](LICENSE).
