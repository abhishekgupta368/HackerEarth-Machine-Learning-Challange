# HackerEarth Machine Learning challenge: Mothers’ Day with Machine Learning

we are all guilty of taking to social media to post mushy messages or images on the second Sunday of May for our mothers. However, the Human Resources team of your organization wishes to celebrate and honor all moms currently employed at the company with a special monthly event. For one of such events, they have reached out to your team to curate and categorize Mothers’ Day-related tweets from across the globe.
As a Machine Learning Engineer, your task is to build a sophisticated sentiment analysis-based NLP model that can classify sentiments of tweets into positive, negative, and neutral.

This project is made for setimential analysis using mothers day dataset of twitter, which will help us to clasify the tweets into three categories:
1. Negative 
2. Neutral
3. Positive

Following Steps followed:

Prepare the NLP pipeline for pre-processing of text.

1. convert string into lowercase.
```
 eg:
   Happy MOTHER days ---> happy mother days
```

2. all the short form word convert to long text.
```
      I'm -> I am
      can't -> cannot
```

3. Words starting with # are removed.
```
  eg:
    #mother
    #happy
```

4. Word starting with @ are removed
```
  eg:
    @abhishek
    @preeti
```

5. All the Http and Https Url are removed from the text
```
 eg:
  https://www.instagram.com
```

6. All the punctations and stopwords are removed.
```
 eg:
   Stopwords: are, is, you, how (They act as noise in string)
   punctuation: .,;'[]{}
   .
```
7. Final Clean text is Obtained:
```
 eg: 
   Happy Mothers days #happy #days @abhi. https://www.google.com/ ---> happy mothers days
```

Prepare Machine Learning Model.

1. After Preprocessing of the text, we will apply TF IDF vectorization to genrate the TFIDF matrix and conver it to 2d Matrix
2. Preprocess the label of the dataset by converting the negative value to postitve like: -1 -> 2
3. I used Navi Bayes Machine learning model for classification as it give me highest accuracy.
4. Predict the output of the test.csv.

