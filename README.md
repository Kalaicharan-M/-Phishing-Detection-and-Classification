⚫ Phishing URL Detection using CNN & CNN-LSTM

This project focuses on detecting **phishing URLs** using **deep learning models**, particularly **Convolutional Neural Networks (CNN)** and **CNN-LSTM hybrid models**, both with and without manual feature engineering.

---

⚫ Problem Statement

Phishing websites trick users into giving up personal information by mimicking legitimate websites. This project aims to classify URLs as **phishing** or **legitimate** based on their structure and characteristics.

---

⚫ Models Used

### Model 1: CNN with Raw URL Input
- Treats URL as a sequence of characters
- One-hot encoding or character-level embeddings
- Captures local patterns (e.g., `https`, `.exe`, long domains)

### Model 2: CNN-LSTM with Raw Input
- CNN for feature extraction + LSTM to capture long-term dependencies
- Suitable for variable-length URL sequences

### Model 3: CNN with Engineered Features
- Input: numeric/categorical features like:
  - URL length
  - Presence of `@`, `//`, IP address
  - Number of subdomains
- Faster training and better interpretability

---

⚫ Feature Engineering (for Model 3)

- `length_of_url`
- `presence_of_https`
- `has_ip_address`
- `num_special_characters`
- `is_shortened_url`
- And more...

---

⚫Evaluation Metrics

All models evaluated on:
- **Accuracy**
- **Precision**
- **Recall**
- **F1 Score**
- **Confusion Matrix**
- **ROC-AUC**

> Example Confusion Matrix:
