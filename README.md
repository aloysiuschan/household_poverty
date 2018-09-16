# household_poverty
The Jupyter notebook contains code to predict poverty level of households in Costa Rica. There are four levels of poverty: extreme, moderate, vulnerable, and non-vulnerable. Features used to predict household poverty include housing characteristics, educational information, and demographic information; missing values were imputed with the column median. I also generated some new variables (e.g. child-to-adult ratio) based on existing variables.

To solve the multiclass prediction problem, I used a random forest classifier, with balanced class weights to address the fact that the target variable had imbalanced classes (the 'non-vulnerable' class dominated the other classes). Cross-validation macro F1 score of the random forest was about 0.40. Average years of education in the household was identified as the most important predictor by the random forest.

The data can be accessed from: https://www.kaggle.com/c/costa-rican-household-poverty-prediction/data
