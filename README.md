Ridge & Lasso Regression Project
=> Introduction
This project is all about exploring regularization in linear regression.
I’ve built two versions of Ridge and Lasso regression:

A manual implementation (without libraries) using gradient descent.

A library-based implementation with scikit-learn, applied to the classic advertising dataset (ad.csv).

The idea is to see how regularization changes the way models learn and how it affects feature importance.

=> Manual Ridge Regression
I started by coding Ridge regression from scratch.

Parameters (w and b) are initialized at zero.

Predictions are made, errors are calculated, and gradient descent updates are applied.

The regularization term (alpha) ensures coefficients don’t grow too large.

This part is a great way to understand what’s happening under the hood.

=> Ridge & Lasso with Libraries
Next, I used scikit-learn to make life easier.

Features: TV, Radio, Newspaper

Target: Sales

I trained both Ridge and Lasso models, evaluated them with Mean Squared Error (MSE) and R² Score, and compared their coefficients.

=> Ridge shrinks coefficients but keeps all features.
=> Lasso can shrink some coefficients all the way to zero, effectively dropping irrelevant features.

=> Visuals
To make things clearer, I plotted the coefficients side by side:

Ridge Regression → All features retained, but shrunk.

Lasso Regression → Some features (like Newspaper) may be eliminated.

This gives a nice visual of how regularization works.

=> Key Insights
Ridge is great when you want to keep all features but control their influence.

Lasso is useful when you suspect some features don’t matter — it performs feature selection automatically.

Regularization helps prevent overfitting and improves generalization.

=> How to Run
Clone the repo and place ad.csv in the same folder.

Install dependencies:

bash
pip install pandas scikit-learn matplotlib
Run the script:

bash
python ridge_lasso.py
Check the console for results and view the plots.

=> Conclusion
This project shows both the math side (manual coding) and the practical side (using libraries) of Ridge and Lasso regression.
It’s a hands-on way to see how regularization shapes models and why it’s such a powerful tool in machine learning.
