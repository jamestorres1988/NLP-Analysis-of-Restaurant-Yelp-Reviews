# Sentiment Classification and Topic Extraction for Restaurants in Cleveland, Ohio

For the presentation, here's a [link.](https://docs.google.com/presentation/d/1hreNKyj12pi_CUPy3Wa4l0SukEB_H3VzRD7iPLcporA/edit?usp=sharing)

We will be using the yelp review dataset for this capstone. Here is the [link](https://www.kaggle.com/yelp-dataset/yelp-dataset/version/6) for the dataset. Due to the size of the dataset, we will filter this dataset to show only restaurants in Cleveland, Ohio. Most restaurant owners will read some or all of their reviews to get a feeling about where their business is going. For restaurants with hundreds of reviews, this can be very difficult. What we hope to do extract keywords from these reviews to provide constructive feedback. This is valuable to restaurant owners because it removes unnecessary guesswork and provides a more detailed means of evaluation besides star ratings. The feedback will consist of 2 parts. First, we will identify positive aspects of the restaurant (i.e. good service, amazing tacos, etc.). Second, we will identify negative aspects of the restaurant. <br/>

The project will be divided into 3 phases over 4 notebooks.

- [Notebook 1, Text Cleaning](https://github.com/jamestorres1988/Final-Capstone/blob/master/Notebook_1_out_of_4_Text_Cleaning.ipynb) (Github)
- [Notebook 2, Phase 1](https://drive.google.com/open?id=1HUpfTqdPWjVU9vTC-GC671OUDByNzOQI) (Best viewed on Google Collab)
- [Notebook 3, Phase 2 & 3](https://drive.google.com/open?id=1c73_l8du7hP3gXlp6V_e0AI1esRAtIQ8) (Best viewed on Google Collab)
- [Notebook 4, Topic Extractor Demo](https://drive.google.com/open?id=1m9wZ4mi-ZrhShA8i1PtAoTCTritrekA9) (Best viewed on Google Collab)

For phase 1, we will divide the reviews into positive and negative reviews. To do this, we would first need to perform sentiment analysis on the Yelp reviews. We will apply a supervised learning approach to perform this using the star rating system to train the data. The reason that we are performing sentiment analysis is that we want to allow this model to be expandable to reviews that do not have star ratings such as Twitter or Facebook comments. The goal is to have a fitted model that can predict sentiment of unlabeled reviews. Importing a Twitter or Facebook dataset is outside the scope of this capstone. Instead, we will perform a train/test split on the yelp reviews, then run several supervised learning models (i.e. random forest, logistic regression, etc.) and compare them. For phase 2, we will then apply our trained sentiment classifier to yelp tips, which are unlabelled. Once we do label the yelp tips, we will then integrate the yelp tips into our dataset. <br/>

For phase 3, we will perform topic modeling on the positive and negative reviews separately. Our goal is to find keywords from each to give us our positive and negative feedback. We will have to decide which text extraction method (BoW or tf-idf) and which dimensionality reduction (LSA, NNMF, or LDA) will make sense for this project. Once we decide on a text extraction method, we will run a demo to see what insights we can get on a specific restaurant. Parts of phase 3 were inspired by a [github](https://github.com/Vishwacorp/yelp_nlp) by Ankur Vishwakarma. Although the general idea is similar, our execution, topics, and conclusion will be different.  


