# Salary Predictive Model

This model was developed using Python v 3.7.6 with the following libraries:
- Scikit-Learn v 0.22.1
- XGBoost v 1.1.0
- Pandas
- Numpy
- Matplotlib
- Seaborn
- Pickle

The primary motivations for this project were to familiarize myself with data cleaning and to practice with different modeling methods. I was particularly interested in working with the XGBoost library and spent a lot of time familiarizing myself with the different hyperparameters and optimizing my tuning method.

The final model is the xgb_salary_predict pickle file. This can be exported and used to predict a salary with similar features. The full breakdown of my cleaning, analysis, and various model tuning can be reviewed in the first_project jupyter notebook. 

Ultimately, this model used the following features to predict a salary:
- A job type (CEO, VP, Manager, Senior, Junior, etc.)
- A degree (High School, Masters, None, etc.)
- A major for that degree, if any
- The job industry
- Years of Experience in the field
- The job's distance (in miles) from a major city

I used sklearn.StandardScalar to normalize my continuous features (yearsExperience and milesFromMetropolis) and pandas.get_dummies to one-hot-encode the remaining categorical features. I used the model's mean-squared-error (MSE) to determine it's accuracy, along with the r-squared value. 

I started with a simple Linear Regression as my baseline model. After detemining it's MSE, I attempted to improve it with a Ridge Regression, Support Vector Regression, and XGB Regression. The XGB model won out with an MSE of ~353, and an r-squared of ~0.765.

Any questions or further discussion please feel free to reach out via email or LinkedIn. I am always open for new ideas to improve and would enjoy expanding our networks.

Email - kohara91@gmail.com
LinkedIn - https://www.linkedin.com/in/kevinodata/
