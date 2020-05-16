# Machine Learning: microlending analysis in Latin America
## Kiva Crowdfunding


This notebook is an extract of a project that was elaborated in collaboration with _Anwesha Tomar, Caroline Sklaver, and Andrea Piolini_. 
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

## 
