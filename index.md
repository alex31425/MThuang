# Article
---
## Python Basics & Cheat Sheets

<figure>
    <img src="images/Python basic.png?raw=true"/>
    <figcaption><a href="https://content.techgig.com/how-to-learn-python-programming-effectively/articleshow/76188658.cms">Image source</a></figcaption>
</figure>
<br>

Python has become one of the most popular open source programming languages. Many powerful libraries that Python support have made a popular choice for data analysis tasks.
There are four most commonly used Python libraries for data analysis : [NumPy](https://numpy.org/), a library for a variety of mathematical and statistical operations ; [pandas](https://pandas.pydata.org/), a library created specifically to facilitate working with data ; [Matplotlib](https://matplotlib.org/), a visualization library that makes it quick and easy to generate charts from data ; [scikit-learn](https://scikit-learn.org/stable/), The most popular library for machine learning work in Python.<br />
<br>
This article introduces Python’s built-in data manipulation tools whcih is helpful to understand Python's add-on libraries like pandas and NumPy for advanced computational functionality for larger datasets.

[Read more](https://alex31425.github.io/MTHuang/Python_Basics_Cheat_Sheets)



---

## Exploratory Data Analysis

- [Data Normalization for Numeric features](https://alex31425.github.io/MTHuang/sample_page)
<br>
<figure>
    <img src="images/data_normalization.jpg?raw=true"/>
    <figcaption><a href="https://www.import.io/post/what-is-data-normalization-and-why-is-it-important/">Image source</a></figcaption>
</figure>
<br>


---
- [Outliers](https://medium.com/analytics-vidhya/detecting-outliers-using-box-and-whisker-diagrams-and-iqr-346a1b9c0dbe)
<br>
<figure>
    <img src="images/outliers.jpg?raw=true"/>
    <figcaption><a href="https://www.rapidinsight.com/blog/handle-outliers/">Image source</a></figcaption>
</figure>
<br>

- [How to Make Your Machine Learning Models Robust to Outliers](https://heartbeat.fritz.ai/how-to-make-your-machine-learning-models-robust-to-outliers-44d404067d07)

---

## Feature Selection & Engineering 
- [The Art of Finding the Best Features for Machine Learning](https://towardsdatascience.com/the-art-of-finding-the-best-features-for-machine-learning-a9074e2ca60d)
- [Feature Selection in Python](https://medium.com/towards-artificial-intelligence/feature-selection-in-python-predictive-hacks-8805b136955e)
- [Preprocessing: OneHotEncoder() vs pandas.get_dummies](https://albertum.medium.com/preprocessing-onehotencoder-vs-pandas-get-dummies-3de1f3d77dcc)
- [5 Concepts Every Data Scientist Should Know](https://towardsdatascience.com/5-concepts-every-data-scientist-should-know-16c74d080a83)
- [Features Engineering: behind the scenes of ML algorithms](https://medium.com/datadriveninvestor/features-engineering-behind-the-scenes-of-ml-algorithms-e356e38073d)

---
## Evaluation Metrics Machine Learning
- [Confusion Matrix](https://towardsdatascience.com/understanding-the-confusion-matrix-and-its-business-applications-c4e8aaf37f42)
- [AUC - ROC Curve](https://towardsdatascience.com/understanding-auc-roc-curve-68b2303cc9c5)



---
## Machine Learning Models

<figure>
    <img src="images/ML.jpeg?raw=true"/>
    <figcaption><a href="https://towardsdatascience.com/machine-learning-for-beginners-d247a9420dab">Image source</a></figcaption>
</figure>
<br>

Before building machine learning models, it is important to prepare data prior to modeling. This may involve replacing missing values, scaling numerical values, and one hot encoding categorical data. Data transforms can be performed using the scikit-learn library; for example, the SimpleImputer class can be used to replace missing values, the MinMaxScaler class can be used to scale numerical values, and the OneHotEncoder can be used to encode categorical variables. The [ColumnTransformer](https://scikit-learn.org/stable/modules/generated/sklearn.compose.ColumnTransformer.html) is a class in the scikit-learn Python machine learning library that allows you to apply data preparation transforms. The categorical and numerical columns is first being identified and then use ColumnTransformer to transfer data. Second, use [sklearn.model_selection train_test_split](https://scikit-learn.org/stable/modules/generated/sklearn.model_selection.train_test_split.html) to split arrays into train and test subsets. We are ready to build the machine learning models. Here are some models that commonly used to train and test the data.
 
[Read more](https://alex31425.github.io/MTHuang/Machine_Learning_models)


---
# Project
### [Machine Learning Engineering for Predicting Major League Baseball Team Wins](https://github.com/alex31425/BDA696-MuTing/wiki)
<br>
<figure>
    <img src="images/project baseball.jpg?raw=true"/>
    <figcaption><a href="https://www.techrepublic.com/article/throwing-a-fastball-how-the-minnesota-twins-are-using-machine-learning-to-analyze-mounds-of-data/">Image source</a></figcaption>
</figure>
<br>
Statistics play an important role in baseball which makes comparisons between players on field performance easy, and these combined statistics can also evaluate each team overall performance for a given days. In this project, I used a historical dataset on a Major League Baseball (MLB) to derive meaningful insights into player and team performance and apply machine learning algorithms to project the a game result. This work analyzes the pitch and batter data with decision tree model, random forest model, K-Nearest model, Kernel SVM, and XGBoost model to study what factors would affect the teams’ performance.
<br>

### [Analysis of Airbnb Lodging Service in San Diego](https://sites.google.com/sdsu.edu/bda594bairbnbanalysis/home)
<br>
<figure>
    <img src="images/airbnb.jpg?raw=true"/>
    <figcaption><a href="https://www.irishtimes.com/life-and-style/travel/airbnb-s-future-depends-on-a-post-pandemic-travel-boom-1.4238881">Image source</a></figcaption>
</figure>
<br>
Airbnb is an online rental marketplace that allows hosts to post their properties for short-term rental. Airbnb logging service has revolutionized the hotel industry and played a key role in our sharing economy. Hosts have to keep monitoring the market, so they do not set the prices too high or too low.  Therefore, hosts need tools to help them price their property more conveniently and sufficiently. This analysis includes data analysis using data visualization on important features such as location and date and 5 different machine models (Simple linear regression, multiple linear regression model, Polynomial Linear regression model, decision tree regressor, Random Forest regression model, and XGBoost model), and compare which models can best predict the price. 
I am responsible for build the machine learning models to conduct predictive analytics which predicts the rental price.

[Download report](/pdf/project_report_1.pdf)
<br>
[Code](https://nbviewer.jupyter.org/github/alex31425/GEOG594-MTHuang/blob/2bf57d19de627d5526f712c3198273376a726b2e/BDA594-combined.ipynb)

<!-- Remove above link if you don't want to attibute -->
