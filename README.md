## Executive Summary

Understanding customer sentiment and its causes at scale is crucial for building a competitive advantage in business. This project applies deep learning models to predict McDonald’s Yelp review ratings and uses explainable AI techniques to identify key words that influence these ratings.

### Problem Definition

Accurate sentiment analysis of customer reviews is key for gaining insights into customer satisfaction and improving business strategies. The challenge is to predict review ratings based on text data. This project leverages natural language processing (NLP) techniques and machine learning models to predict Yelp review ratings and understand the factors influencing these ratings.

## Data Sources

- **Yelp Dataset**: Contains ~17K reviews of McDonald's spanning from 2007 to 2022.
- **Additional Data**: Text data processed using various NLP techniques to extract meaningful features for modeling.

## Methodology

- **Data Cleaning**:
  - Removed special characters, punctuations, and white space.
  - Tokenization: Split text into individual tokens.
  - Stop Words: Removed common words that may not carry significant meaning.
  - Lemmatization: Reduced words to their base or root form.

- **Modeling**:
  - **Feature Engineering**: Created features using TF-IDF and focused on binary classification for 1 and 5 star reviews.
  - **Model Selection**: Evaluated logistic regression, Naïve Bayes, and deep learning models (including LSTM).
  - **Performance Metrics**: Accuracy, F1 Score, Recall, and Precision were used to evaluate model accuracy.

## Lessons Learned

- **NLP**: Text data requires extensive preprocessing and feature extraction before modeling. Deep contextual understanding (e.g., BERT) can improve model performance but may have computational constraints.
- **Deep Learning**: Explainable AI (XAI) techniques provide interpretability, but results from Lime and SHAP were less insightful than expected.

## Future Work

- **Improve Overfitting**: Despite regularization and reducing model complexity, overfitting persisted.
- **Aspect-Based Sentiment Analysis (ABSA)**: Prioritize sentiment analysis related to specific aspects such as food quality and service.
- **Sentiment Trend Analysis**: Analyze sentiment trends over time and correlate them with external factors like new menu items or promotional campaigns.
- **Dataset Expansion**: Expand the dataset to include reviews from other platforms like Google Reviews and Reddit.
