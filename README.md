# Machine Learning: microlending analysis in Latin America
## The case of Kiva Crowdfunding

The aim of the project is to gain insight into how Kiva.org, an online crowdfunding platform that extends financial services 
to poor people, determines the repayment interval (monthly, bullet or irregular) of each loan granted in Latin America. The
aim was also to determine which features play an important role when it comes to determining the repayment intervals and whether
the Multidimensional Poverty Index has an effect on the loans repayment conditions. 

**Machine Learning algorithms** were applied to predict the repayment interval (categorical variable with 3 classes) 
based on features such as gender, number of lenders, economic activity, number and gender of borrowers, etc.

After a basic **preprocessing of the data** (choose identifiers, handle missing data, identify categorical variables and 
remove outliers), a test, validation, and training sets were created. **Hyperparameter tuning** was performed over different 
models (including: **Logistic Regression, Random Forest, Decision Trees, Hgbc, Xgboost, and Multilayer Perceptron**). 
Afterwards, the best model was selected based on the parameter scores. Finally, the features with the most **information gain** 
were exlpored.

## About the source

The dataset was obtained from [kaggle](https://www.kaggle.com/ishaanmalhi/kiva-org-microlending-analysis-and-prediction).
The Multidimensional Poverty Index (MPI) was obtained from the United Nations Development Program [website.](http://hdr.undp.org/en/2018-MPI)

## About the project

This notebook is an extract of a project that was elaborated in collaboration with _Anwesha Tomar, Caroline Sklaver, and Andrea Piolini_. The project was part of an assignment from Machine Learning 1 class at GWU in Spring 2020. Python 3.7.4 was used for data analysis. **Pandas** and **Numpy** were used for preprocessing. **Sklearn** was used for applying machine learning algorithms.

## Key findings

- There is a strong positive correlation between the number of female borrowers and loan amount, as the correlation plot suggests.
- Term in months is the feature with the most predictive power for determining the interval payment in Latin America.
- Loans granted for agriculture and livestock activities is also an important feature with high predictive power. As depicted in the correlation matrix, there is a strong positive correlation between financed agriculture activies and male borrowers.
- Histogram Gradient Boosting Classifier (with a learning rate of 0.1) proved to be the model with the highest score; followed by Xgboost and Random Forest.
- The Multidimensional Poverty Index of a country is the fourth feature with the most information gain.

