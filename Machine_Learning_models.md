Before building machine learning models, it is important to prepare data prior to modeling. This may involve replacing missing values, scaling numerical values, and one hot encoding categorical data. Data transforms can be performed using the scikit-learn library; for example, the SimpleImputer class can be used to replace missing values, the MinMaxScaler class can be used to scale numerical values, and the OneHotEncoder can be used to encode categorical variables. The [ColumnTransformer](https://scikit-learn.org/stable/modules/generated/sklearn.compose.ColumnTransformer.html) is a class in the scikit-learn Python machine learning library that allows you to apply data preparation transforms. The categorical and numerical columns is first being identified and then use ColumnTransformer to transfer data. Second, use [sklearn.model_selection train_test_split](https://scikit-learn.org/stable/modules/generated/sklearn.model_selection.train_test_split.html) to split arrays into train and test subsets. We are ready to build the machine learning models. Here are the models I am going to train and test the data.
 
* [Decision Tree Classifier](https://scikit-learn.org/stable/modules/generated/sklearn.tree.DecisionTreeClassifier.html#sklearn.tree.DecisionTreeClassifier) \
Decision tree algorithms work by constructing a “tree.” A decision tree is a supervised machine learning algorithm that can be used for both classification and regression problems. A decision tree is simply a series of sequential decisions made to reach a specific result. Decision trees over other machine learning algorithms is how easy they make it to visualize data.\



* [Random Forest Classifier](https://scikit-learn.org/stable/modules/generated/sklearn.ensemble.RandomForestClassifier.html)\
Random Forest is a tree-based algorithm that randomly creates decision trees. The random forest then combines the results of each random tree to generate the final output. Random forests are commonly reported to have higher accuracy than other learning algorithms.\



* [XGBoost](https://xgboost.readthedocs.io/en/latest/)\
XGBoost is termed as Extreme Gradient Boosting algorithm works by boosting trees and makes use of a gradient descent algorithm which is the reason that it is called Gradient Boosting. XGBoost uses a continuous score assigned to each leaf which is summed up and provides the final prediction. This allows the algorithm to sequentially grow the trees and learn from previous iterations. The whole idea is to correct the previous mistake done by the model, learn from it and its next step improves the performance. The previous results are rectified, and performance is enhanced.\


* [KNeighbors Classifier](https://scikit-learn.org/stable/modules/generated/sklearn.neighbors.KNeighborsClassifier.html)\
k-nearest neighbors algorithm (KNN) can be used for classification and regression problems. The KNN algorithm assumes similar things are near to each other. In other words, it assumes the similarity between the test data and training data and put the test data into the category that is most similar to the available categories.\
The accuracy rate (53%) for the KNeighbors model is the highest among these models. 



* [Support Vector Machines](https://scikit-learn.org/stable/modules/svm.html)\
Support Vector Machines (SVM) is a learning algorithms that analyze data for classification and regression analysis.Support Vector Machines outputs an optimal line of separation between the classes based on the training data served as input. This line of separation is called a hyperplane in a multi dimensional environment.\


- [Machine Learning Models Explained to a Five-year-old](https://towardsdatascience.com/machine-learning-models-explained-to-a-five-year-old-f2f540d9dcea)
- [Data Science Concepts Explained to a Five-year-old](https://towardsdatascience.com/data-science-concepts-explained-to-a-five-year-old-ad440c7b3cbd)
- [5 Machine Learning Regression Algorithms You Need to Know](https://medium.com/analytics-vidhya/5-regression-algorithms-you-need-to-know-theory-implementation-37993382122d)
