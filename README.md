# genre_classification_and_bpm_prediction
R project for song genres classification and tempo (BPM) prediction

The goal of the project was to predict genres and the beat/tempo of songs according to the frequency and energy over time. 

I was assigned two datasets, one for prediction the tempo and another for the genre classification:

Tempo: 20 observations and 96 variables
Genre: 150 observations, 5144 variables and 5 classes for the response variable ('country', 'hiphop', 'metal', 'reggae', 'rock')

The problem was tricky, since it was provided a very complex, high dimensional and sparse (almost 70%) dataset. The main issue of both cases was the variable selection to reduce the dimension of the problem.

For the regression problem, I used LASSO, Ridge and Elastic Net (model that balances the penalties between LASSO and Ridge). I selected the model through Leave-One-Out Cross Validation (LOOCV), since there wouldn’t be computational issue, since the number of observations was small.

In the genre classification, among the models used are: Random Forest, Naive Bayes, boosted logistic regression and GLMNET.

Keywords: R, High Dimensionality and Sparsity, LASSO, Ridge Random Forest, Naive Bayes
