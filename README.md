# Sentiment Analysis - Movie Reviews
The purpose of the current project is to train and test a Machine Learning model able to classify movie reviews either as *positive* or *negative*.
The notebook is structured as follows:
- Data Overview
- Preprocessing
- Modelling
- Testing
## Data Overview
The data\* is stored in a structured directory, described below.
```
movie_reviews/
  neg/
  pos/
```
Each subdirectory, `neg/` and `pos/`, contains multiple .txt files with reviews.

## Preprocessing
This phase includes the cleaning and formatting the data before training a model. The computers are not good understanding raw text, then this process converts the text to a vector which is "understadable" by the computer. The following steps will be followed on purpose.
- Lowercasing
- Tokenizing
- Removing stop words and punctuation

The data have been partly normalized at this point. Before we continue preprocessing the data we will build up a *WordCloud\** which will give us an idea of the most common words in the `movie_revies.data`.

Then, the preprocessing phase will continue with the following steps.
- Stemming
- Vectorizing
\**The WordCloud is not considered as a preprocessing step because it will not change or process the data, it will give us an idea of the most common words in the reviews.*

## Modelling
This section is composed by rhe following two steps. 
- Train Test Set Split
- Training
    - Naive Bayes
    - Support Vector Machine
    - Logistic Regression
    - Random Forest
- Error Analysis
    - Acurracy
    - Classification Report
    - Confusion Matrix
    - Precision - Recall
    - ROC Curve

## Testing
The chosen model was tested with the [Rocky 4 Reviews - Rotten Tomatoes](https://www.rottentomatoes.com/m/rocky_iv/reviews/?type=user).
