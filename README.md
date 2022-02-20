# una-hw
In this assignment, we want to explore whether GraphSage algorithms can help in improving predictions for training machine learning models on Yelp dataset.

We are going to train traditional Machine Learning and Deep Learning models by categories of restaurants and attributes of users and predict results of 5 ordinal labels: 1, 2, 3, 4, 5. 
At first, we predict rating by traditional Machine Learning and Deep Learning models and get (test) accuracy of 40% and 45$ separately.
Then we convert training data with over 1000 categorical features into graph embeddings of 40 dimensions, pass into previous models and accuracy decreases to (test)48% and 62%.In order to train graph model, we treat reviews as nodes and link those with same user_id and business_id.

So GraphSage help the predictions a little bit since it compress over 1000 sparse categorical features into 40 dimensions. This is especially true when we amount of nodes is very limited. Besides, decrease from training accuracy to test accuracy also reduces a lot(ML model: 53%/40% -> 49%/45%, DL model: 53%/48%->63%/62%) with graph embeddings, which means algorithm has also been stabilized. 
