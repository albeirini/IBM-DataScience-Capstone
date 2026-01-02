## Snippet to scale and standardize the data

from sklearn import preprocessing
scaler = preprocessing.StandardScaler()
X=scaler.fit_transform(X)

Standardization was applied to ensure all features contribute equally to model training.

## Snippet to showcase the function train_test_split

X_train, X_test, Y_train, Y_test=train_test_split(X,Y,test_size=0.2,random_state=2)

The dataset was split into 80% training and 20% testing data.

## Snippet to show GridSearch object with Logistic Regression.

from sklearn.linear_model import LogisticRegression
from sklearn.model_selection import GridSearchCV

parameters ={'C':[0.01,0.1,1],
             'penalty':['l2'],
             'solver':['lbfgs']}

parameters ={"C":[0.01,0.1,1],'penalty':['l2'], 'solver':['lbfgs']}# l1 lasso l2 ridge
lr=LogisticRegression()
logreg_cv=GridSearchCV(estimator=lr,param_grid=parameters,cv=10)
logreg_cv.fit(X_train,Y_train)

GridSearchCV was used to tune hyperparameters and select the best-performing model.

## Snippet to show calculation of model accuracy

Logreg_score=logreg_cv.score(X_test,Y_test)
Logreg_score

Model accuracy was evaluated using the .score() method on the test dataset.