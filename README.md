# Recommendations with IBM

# Installation
The libraries/packages used are:

- numpy
- pandas
- matplotlib
- pickle

# Project Motivation
The project is the third project for the [Udacity Data Scientist Nanodegree](https://www.udacity.com/course/data-scientist-nanodegree--nd025) - Term2. 

The goal for this project is to analyze the interactions that users have with articles on the IBM Watson Studio platform and make recommendations to them about new articles that they will like. 

# File Descriptions
- This notebook `Recommendations_with_IBM.ipynb` includes the process of exploratory data analysis, rank based recommendations, user-user based collaborative filtering, and matrix factorization.
- `Recommendations_with_IBM.html` is the HTML output of the `Recommendations_with_IBM.ipynb` juypter notebook
- `user_item_matrix.p` is a pickle file used in the matrix factorization step
- `top_5.p`, `top_10.p`, `top_20.p` and `project_tests.py` are the test files to test the result of the jupyter notebook.
- `data` folder: `articles_community.csv` is the article details on IBM Watson Studio. `user-item-interactions.csv` is the user and article interaction file.

# Results
The project explores the user data on the IBM Watson Studio platform and applied three recommendation techniques: rank based recommendations, user-user based collaborative filtering, and matrix factorization.

The result for matrix factorization method is not great due to below reasons:

- The user overlap between the training set and the test set is too small.
- There are too many zeros in the test set. The result above shows that if we predict all zeros (null model), the accuracy rate is the highest.
- The cost function that we want to minimize (err) might not be a good idea since it is not meaningful to predict all zeros.

# Licensing, Authors, Acknowledgements
1. Credits to https://github.com/paawan01/Titanic_dataset_analysis for the readme template

