# Project 3

Posted: November 2, 2017

Due: November 17, 2017

This project focuses on utilizing the NLP skills we learned to do two basic text analysis tasks. Although the text below references NLTK, you are free to use any other NLP package instead (e.g., spaCy).

## Part 1: Review Classification

This part uses the Amazon Fine Foods reviews dataset, that contains reviews for a collection of products from Amazon. You can find the full dataset at: https://snap.stanford.edu/data/web-FineFoods.html. The project directory contains a small portion of it (not a random sample) with 2000 reviews. The format of the file should be self-explanatory. 

Your task is to read in this file, and construct a simple classifier to predict the `review/score` from the `review/userId`, `review/profileName`, `review/time`, `review/summary`, and `review/text` (but not the `productId`, or `helpfulness`). You should figure out different types of features to use for this task, and should use a Naive Bayes Classifier for the classification (you can use other methods if you'd like). You should use off-the-shelf implementation -- here is the sci-kit one: http://scikit-learn.org/stable/modules/naive_bayes.html

(Optional) As an optional task, try to predict the `review/helpfulness` from the rest of the information (including the `review/score`). Note that, modeling time would be crucial here, since later reviews are less likely to be voted as helpful or unhelpful.

## Part 2: Named Entity Recognition

Here, we will use the Named Entity Recognition functionality of NLTK to extract entities and relationships from some recent news articles. Specifically, pick your favorite viewer sport (football, soccer, tennis, baseball, cricket, etc.), and download 10 recent news articles describing some games/matches (e.g., http://www.npr.org/sections/thetwo-way/2017/11/01/561445201/it-s-winner-take-all-in-game-7-of-the-world-series). 

Use NLTK to write code to extract named entities from each of them. The final output should simply be a list of entities and their types, which would require understanding the structure of the output of the `ne_chunk` command, and traversing it to find just the named entities.

Next, write a few regular expressions to extract information about which `positions` or `roles` different players serve in their team. For example, from the above link, the sentence `The Dodgers put their leadoff hitter, Forsythe, on base with a single.` tells us that: `Forsythe` is the `leadoff hitter` for `Dodgers`. The regular expression that you write here will be specific to the sport that you have picked.

## Submission

Submit a zip file containing your Jupyter notebook as well as the text of the 10 articles that you downloaded for the second part.
