# Personalize Expedia Hotel Searches
![Screen Shot 2021-12-20 at 19 58 07](https://user-images.githubusercontent.com/41892953/146868586-67ba9ae0-f7b7-454b-982e-1d37f9b9e74d.png)

## Problem Statement
[Expedia](https://www.expedia.com/) is the world’s largest online travel agency (OTA) and powers search results for millions of travel shoppers every day. In this competitive market matching users to hotel inventory is very important since users easily jump from website to website. As such, having the best ranking of hotels (“sort”) for specific users with the best integration of price competitiveness gives an OTA the best chance of winning the sale.

For this [contest](https://www.kaggle.com/c/expedia-personalized-sort/overview), Expedia has provided a dataset that includes shopping and purchase data as well as information on price competitiveness. The data are organized around a set of “search result impressions”, or the ordered list of hotels that the user sees after they search for a hotel on the Expedia website. In addition to impressions from the existing algorithm, the data contain impressions where the hotels were randomly sorted, to avoid the position bias of the existing algorithm. The user response is provided as a click on a hotel or/and a purchase of a hotel room.

## Libraries
- scikit-learn
- XGBoost
- Pandas
- Numpy

## Files
- [`Expedia_learning_to_rank_with_parameter_tuning.ipynb`](https://github.com/wmingch1992/Expedia-Learning-to-rank/blob/main/Expedia_learning_to_rank_with_parameter_tuning.ipynb) built a machine learning-to-rank model using [XGBoost](https://xgboost.readthedocs.io/en/stable/).

## Results 
- The evalution metric for this competiion is [Normzlied Discounted Cumulative Gain](https://towardsdatascience.com/normalized-discounted-cumulative-gain-37e6f75090e9) (NDCG@38) 
- The private score is 0.50340 (ranked 49/336, top 14.6%)

## Next step
- The results could be further improved by tuning the XGBoost hyperparameters 
- train a meta-model on top of XGBoost, lightGBM and Catboot learning to rank models
