**Project Summary: Sentiment Analysis of IMDB Movie Reviews**

This project aimed to perform sentiment analysis on a substantial dataset of IMDB movie reviews. It involved various stages, from data acquisition to model tuning, and led to the development of a sentiment analysis model with high accuracy.

**Key Steps in the Project:**

1. **Data Query from IMDB Database**: The project commenced with querying and extracting data from the vast IMDB database. This step ensured access to a diverse set of movie reviews.

2. **Initial Visualization with Looker**: Initial data exploration and visualization were carried out using Looker. This provided a preliminary understanding of the dataset and allowed for high-level insights into the content of the movie reviews.

3. **Further Data Preparation and Exploration**:
   - **Word Cloud**: Word cloud visualizations were created to identify frequently occurring terms in the movie reviews. This offered insights into the most common words used by reviewers.
   - **Word Counts**: The project involved analyzing word counts to assess the length and complexity of movie reviews.
   - **Sentiment Analysis**: Sentiment analysis was performed to classify reviews into positive and negative sentiments. This step helped gauge the overall sentiment distribution.

4. **Data Tokenization**: The text data underwent tokenization, where it was split into individual words or tokens. Tokenization is a fundamental step in natural language processing.

5. **Stemming and Lemmatizing**: Words were stemmed and lemmatized to reduce inflected words to their root forms. This process streamlined the text data for further analysis.

6. **Text Transformation with Lexicon-based Transformer**: A standard text transformer, relying on lexicon-based sentiment analysis, was employed. This approach achieved a moderate accuracy level of around 67% in classifying reviews accurately.

7. **Model Tuning with Different Algorithms**:
   - **XGBoost**: The project explored the XGBoost algorithm for sentiment analysis. With parameter tuning, the XGBoost model achieved notable results.
   - **Multinomial Naive Bayes (NB)**: Multinomial Naive Bayes was employed and tuned, yielding the best performance with up to 87% of reviews accurately classified.
   - **Random Forest (RF)**: The Random Forest algorithm was also tested and tuned to enhance its accuracy.

**Conclusion and results:**

### ROC Curve Analysis
![ROC Curves](/ROC_curves.png)

The Receiver Operating Characteristic (ROC) curves were used to evaluate the performance of different models in the sentiment analysis of movie reviews. The ROC curves visually represent the trade-off between the True Positive Rate (Sensitivity) and the False Positive Rate (1 - Specificity) for each model.

- **Multinomial Naive Bayes (AUC = 0.87)**: The ROC curve for the Naive Bayes model showed strong performance with an AUC of 0.87. This indicates a high ability to distinguish between positive and negative sentiment in movie reviews.

- **XGBoost Classifier (AUC = 0.86)**: The ROC curve for the XGBoost model demonstrated good performance with an AUC of 0.86. It showcases the model's ability to classify sentiments effectively.

- **Random Forest Classifier (AUC = 0.85)**: The ROC curve for the Random Forest model displayed respectable performance with an AUC of 0.85. It suggests a reasonable capability to categorize movie reviews based on their sentiment.

### Confusion Plots

![Confusion Plots](/Conf_mats.png)

In this project, we conducted sentiment analysis on movie reviews using three different machine learning models: Multinomial Naive Bayes, XGBoost, and Random Forest Classifier. We assessed their performance and selected the best model based on accuracy, precision, recall, and F1-score.

## Conclusion

In the process of tuning all the models, Multinomial Naive Bayes emerged as the best performer with an accuracy of 87%. Its efficiency in training and inference, owing to the mathematical foundations of the model, makes it a clear winner for scalability and real-time applications. It provides balanced classification of positive and negative sentiments.

XGBoost, while a close second with an accuracy of 86%, demonstrates excellent precision and recall for both classes.

Random Forest Classifier also offers competitive performance, with an accuracy of 85%.

In conclusion, the choice of the best model depends on specific project requirements, but Multinomial Naive Bayes offers a strong candidate for movie review sentiment analysis.