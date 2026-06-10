# Phishing URL Detector

A machine learning-based cybersecurity project that detects phishing URLs using engineered lexical and structural URL features. The project compares Logistic Regression, Random Forest, and LightGBM classifiers to identify the most effective approach for malicious URL detection.

## Dataset

- Dataset: Websites Dataset
- Size: ~120,990 URLs
- Task: Binary Classification (Phishing vs Legitimate)

## Feature Engineering

Raw URLs were transformed into machine learning features including:

- URL length
- Domain length
- Number of digits
- Number of special characters
- Number of dots and hyphens
- Subdomain count
- HTTPS usage
- Suspicious keyword indicators
- Structural URL characteristics

## Models Evaluated

- Logistic Regression
- Random Forest
- LightGBM

Models were compared using ROC-AUC, PR-AUC, Precision, Recall, and F1-score.

## Results

| Model | ROC-AUC | PR-AUC |
|---------|---------|---------|
| Logistic Regression | 0.9186 | 0.8434 |
| Random Forest | 0.9907 | 0.9762 |
| LightGBM | **0.9932** | **0.9817** |

**Best Model:** LightGBM

The final model was further optimized through hyperparameter tuning, probability calibration, and threshold optimization to improve phishing detection performance.

## Tech Stack

- Python
- Pandas
- NumPy
- Scikit-learn
- LightGBM
- Matplotlib
- Jupyter Notebook

## Future Work

- Real-time phishing detection API
- Browser extension integration
- Deep learning-based URL classification
- Explainable AI for phishing prediction
