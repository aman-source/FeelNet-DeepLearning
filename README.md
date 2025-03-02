# FeelNet-DeepLearning
A deep learning-based emotion classification model that analyzes text-based interactions, including customer reviews and feedback. The project explores multiple approaches, including Logistic Regression (TF-IDF), CNN, and LSTM, to detect emotions such as joy, sadness, anger, fear, love, and surprise. LIME is used to interpret model decisions and improve explainability.


## Overview
This project builds an emotion classification model using three different approaches:
1. **Logistic Regression (TF-IDF)**
2. **CNN (Word Embeddings)**
3. **LSTM (Word Embeddings)**

The models are evaluated using precision, recall, F1-score, and accuracy. LIME is used to explain model predictions.

## Dataset
- The dataset contains text samples labeled with emotions such as joy, anger, sadness, fear, love, and surprise.
- Preprocessing steps include tokenization, stopword removal, lemmatization, and padding for deep learning models.

## Models Implemented
### 1. Logistic Regression
- Uses TF-IDF vectorization for feature extraction.
- Simple and interpretable model.

### 2. Convolutional Neural Network (CNN)
- Uses word embeddings as input.
- Captures local word patterns.

### 3. Long Short-Term Memory (LSTM)
- Captures sequential dependencies in text.
- Suitable for complex patterns in emotions.

## Model Interpretation with LIME
LIME is used to explain the predictions by highlighting the most influential words in a given text. The explanation helps in identifying which words contributed the most to a particular classification.

## Results
| Model  | Accuracy |
|--------|----------|
| Logistic Regression | 87% |
| CNN                 | 91% |
| LSTM                | 35% |

CNN performs the best, while LSTM underperforms and requires tuning.

## Next Steps
- Fine-tune hyperparameters for better performance.
- Explore ensembling techniques to improve results.
- Deploy the best model using FastAPI or Flask.
- Implement real-time monitoring with MLflow.


## Contributors
- Aman Alisha Shaik

## License
This project is open-source and available under the MIT License.
