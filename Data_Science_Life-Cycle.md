[![Data_Science_lifecycle](images/Data_Science_lifecycle.png)](https://alex31425.github.io/MTHuang/images/Data_Science_lifecycle.png?raw=true){:target="_blank"} 
<figcaption><a href="https://docs.microsoft.com/en-us/azure/machine-learning/team-data-science-process/lifecycle">Image source</a></figcaption>{:target="_blank"} 

<br>
Nowadays data science is a trending topic. When a data scientist is starting a data science project, there are a few stpes that normally need to follow in order to complete a project. In this article, I will walk you through these steps and learn how to do a data science project by follwoing these steps. These steps are not linear process as you can see the above diagram. We may need to run the steps iteratively and find the best models that meet our initial objects. 
<br>
- **Business understanding/problem identification**
<br>
Our ultimate goal is to solve a problem/issue that a company that is facing and needs to come up with a soluation to fix it. Otherwise this problem/issue may ,for example,affect the profit margins or customer satification. Image you work for a bank as a data scientist and that marketing department recently noticed that the number of credit card applications is decreasing compared to the same period last year. Therefore, your task is to find out what factors that may influence the churn rate. 
<br>
Next is to define the project goal. Generally speaking, the goal have two types : continuous(regression) or categorical(classification). For example, what will be the sales amount for the next quarter? This is the regression problem. On the other hand, determin whether this customer would stop using our product is a classification problem : Yes or no.    
<br>

- **Data acquisition/data understanding**
<br>
Once the problem is identified, the data scientists can begin collecting the data. Usually, the data source can be categorized into three types : structured data, semistructured data, and unstructured data. Depends on the data source, the collected data could be one of the type or mix of these three types. [ETL](https://www.talend.com/resources/what-is-etl/)—Extract, Transform, Load—is the process of collecting data from multiple source, transforming that data into a common type, and consolidating it into a single, centralized location. Once the data has been extracted, transformed, and loaded to the data warehouse, we should do the [exploratory data analysis](https://alex31425.github.io/MTHuang/Exploratory_Data_Analysis) in order to analyze data sets to summarize their main characteristics.


- **Feature engineering & Model building**
<br>
Before building the models, we need to transform raw variables to create the features from raw data by using the domain knowledge. This process is known as feature engineering which is an important process to understand how the features relate to each other and feed these features to your models. Informative variables improve the models accuracy. Then, based on the questions we would like to answer, there are many modeling algorithms available. Once the algorithms are chosen, it's time to train the models. First, the dataset needs to be split into training and test datasets. Then we can feed the training dataset to our models and evaluate the models accuracy. This process could be repetitive until we reach the desire result.     


- **Model deployment**
<br>
In the previous step, we have build several models and feed the training to train the models. We used [metrics](https://machinelearningmastery.com/metrics-evaluate-machine-learning-algorithms-python/) to evaluate our models' performances. Finally, the best model is chosen. Let's recall in the step 1, the main goal of models building is to answer the question we defined in the step 1 so the final model should be available for the end-users. Therefore, the model should be deployed and implement it into productions as web-services. There are a variety of web-services available such as [AWS Lambda](https://aws.amazon.com/lambda/), [Google Cloud](https://cloud.google.com/) and [Microsoft Azure](https://azure.microsoft.com/en-us/services/functions/) or to deploy a flask or django application through a docker container (Amazon ECS, Azure Container Instance or Google Kubernetes Engine).



Reference
- [The “Generic” Data Science Life-Cycle](https://towardsdatascience.com/stoend-to-end-data-science-life-cycle-6387523b5afc)
- [Data Science Life Cycle in 5 Steps!](https://medium.com/@vanshikagoel/data-science-life-cycle-in-5-steps-3fe720b2a2fe)
- [The Team Data Science Process lifecycle](https://docs.microsoft.com/en-us/azure/machine-learning/team-data-science-process/lifecycle)
- [Life Cycle of a Data Science Project](https://www.dezyre.com/article/life-cycle-of-a-data-science-project/270)
- [The Data Science Life Cycle](https://www.dezyre.com/article/life-cycle-of-a-data-science-project/270)
- [Overview of Different Approaches to Deploying Machine Learning Models in Production](https://www.kdnuggets.com/2019/06/approaches-deploying-machine-learning-production.html)
- [How to Deploy Machine Learning Models using Flask](https://www.analyticsvidhya.com/blog/2020/04/how-to-deploy-machine-learning-model-flask/)
