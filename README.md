# steam review sentiment analysis (ml project)

## overview

general: project is intended for personal exploration of sentiment classification on steam game reviews using ml techniques.
learning outcomes: understanding text features, class imbalance and model choices and their performance

## dataset

----- NOTE: DUE TO FILE LIMITS THE DATASET IS NOT INCLUDED IN THIS REPOSITORY -----

source: kaggle steam reviews dataset => https://www.kaggle.com/datasets/andrewmvd/steam-reviews

1. download the linked dataset
2. place the raw csv file in 'data/raw'
3. run 01_exploration.ipynb to generate processed data

----- NOTE: DUE TO FILE LIMITS THE DATASET IS NOT INCLUDED IN THIS REPOSITORY -----

fields:
: review_text
: review_score {-1,1}

data was cleaned to remove all empty / invalid reviews

## approach

1. exploratory da
2. text feature engineering using tf-idf
3. creating abaseline logistic regression
4. handling class imbalance and class weight
5. learning evaluation through confusion matrix and f1-score data

## models

: a logistic regression as the baseline
: logistic regression with class weighting as the current

## results

accuracy: ~94%
macro f1 improved over time with different class weighting approaches
negative class recal was improved significantly from initial setup at the cost of minor precision

## limitations

heavy imbalance in dataset
public sourced and unmoderated reviews lead to sarcastic and short reviews, hard to classify
stopword handling required modification to prevent heavy data loss on training

## future work

comparing against naive bayes
threshhold tuning usin predicted probabilities
experimenting with bigrams in a more systematic way
