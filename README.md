# Fake news machine learning

This project classfies the dataset into 2 categories: 
- 0 => Real news
- 1 => Fake news 

We have 5 columns:
1/ id
2/ title
3/ author
4/ text
5/ Label (0 or 1)

For this project, I chose to combine the columns 'title' and 'author' into one column 'title/author' and apply the machine learning model on it instead of choosing the 'text' column because it will take forever to process it.

Luckily, the accuracy was very satisfying. Otherwise, I would have chosen the 'text' column even if it's big.

Since, the ML models don't process strings (or text), I had to convert the text into numerical values (vectorizing) but also process the text by elimating the non relevant words (stopwords library) and filtering the words by finding their root (stemming).

The machine learning model used in this project is LogisticRegression which is a supervised machine learning model used for classification purposes.

PS: here is the link to the dataset in kaggle: https://www.kaggle.com/competitions/fake-news/data?select=train.csv
