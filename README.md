# Generating Mood Playlists

## Framing the Problem

### Business Objective

We would like to improve our approach to recommending music to our users and making better quality playlists that fit a user's different moods. In the long run, we want to do so to increase product value and retain users and market share. This is quite important as we are going against Apple Music, a competiting product that has a considerable portion of market share.

### The Model

To improve our recommendation system and increasing product value, we have to try to understand what is the relationship between a user's mood and a song's audio features. This field of study is called music emotion recognition (MER) and there has been studies in the past that map this relationship through theoretical models. By applying these models and audio features of different songs to machine learning, we try to find mood structure and patterns within the songs. We will use a Gaussian Mixture Model (GMM) clustering approach to do so and analyze the results to label the dataset. We will also be using the BIC score as a way of determining the number of components/clusters we want to have.

After labeling the dataset, we plan to test out 2 different models to classify the dataset based on the mood it evokes. These models are Random Forest, K-Nearest Neighbors and Gradient Boosting. (This is in the works.)

### Performance Assessment

There is no way of measuring the performance of our labeling efforts, but we will analyze the result and compare it according to theoretical studies to validate our results in a non-technical manner.

As for our models used to classify the dataset, we'll be using the F1-score and the area under the precision-recall curve as we would like to classify as many songs by their correct mood as possible to minimize inaccuracy of mood class assignment.

### Assumptions

GMM clustering assumes that the data is of a Gaussian mixture distribution and each song are independent from each other.

For classification, both random forest and gradient boosting are non-parametric models.

Resource: https://www.kdnuggets.com/2021/02/machine-learning-assumptions.html