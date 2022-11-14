# Assignment 4
#### DATA602

Posted: November 14th 2022

Due: December 14th, 2022

This project focuses on *natural language processing (NLP)* by asking you to work on a basic text analysis task. Although the text below references NLTK, you are free to use any other NLP package instead (e.g., spaCy).

## Review Classification

This part uses the Amazon Fine Foods reviews dataset, that contains reviews for a collection of products from Amazon. You can find the full dataset at: https://snap.stanford.edu/data/web-FineFoods.html. The project directory contains a small portion of it (not a random sample) with 2000 reviews. The format of the file should be self-explanatory. 

Your task is to read in this file, and construct a simple classifier to predict the `review/score` from the `review/userId`, `review/profileName`, `review/time`, `review/summary`, and `review/text` (but not the `productId`, or `helpfulness`). You should figure out different types of features to use for this task, and should use a Naive Bayes Classifier for the classification (you can use other methods if you'd like). You should use off-the-shelf implementation -- here is the sci-kit one: http://scikit-learn.org/stable/modules/naive_bayes.html

(Optional) As an optional task, try to predict the `review/helpfulness` from the rest of the information (including the `review/score`). Note that, modeling time would be crucial here, since later reviews are less likely to be voted as helpful or unhelpful.

Tips / Hints: This assignment is intentionally open-ended. You are tasked with both cleaning the given data and extracting the necessary information, as well as implementing a new set of Python packages for NLP (namely SpaCy will be usefule -- please investigate the documentation and example implementations). Specifically, after you have reformatted the data into a table of the values you need, try to determine what information can be obtained from the individual reviews that would be useful in predicting a rating? What language do a positive reviews have in common? What about negative? We are not looking for a top-of-the-line predictive model, but rather that you have experimented with the analyzying *text* data, rather than the usual numerical.

## Submission

Submit your Python notebook as well as a brief explanation of the features you extract / how you get predictive information from the reviews.
