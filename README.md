# Machine learning

With this project I have decided to use Panda as my python library.

The guide I used for my project is linked [here](https://www.w3schools.com/python/python_ml_multiple_regression.asp)

## What model is this based on?

Linear regression is predicting the value of a dependent variable based on the independent variable.

Pandas uses multiple regression as its machine learning model, multiple regression is similar to linear regression however there is more than one independent value.

Multiple regression is a form of supervised learning which is when the algorithm is fed with labelled training data. The labbeled data has the outcome for the inputted data it uses the data to recognize patterns.

### Possible adaptation:

To allow for clustering the model must change its operation by using unserpervised learning instead which does not work as the model uses supervised learning.clustering is similar to the classification model where its aim is to identify patterns and group data seperatly

<img src="https://media.geeksforgeeks.org/wp-content/uploads/20190812011831/Screenshot-2019-08-12-at-1.09.42-AM.png" alt="ML | K-means++ Algorithm - GeeksforGeeks"/>![image](https://user-images.githubusercontent.com/99629727/156688948-7d50ae2c-d780-491c-baad-7ac35e02f45a.png)

<img src="https://sweetcode.io/wp-content/uploads/2019/02/pasted-image-0-1.png" alt="From Simple to Multiple Linear Regression with Python and scikit –  Sweetcode.io"/>![image](https://user-images.githubusercontent.com/99629727/156689098-73fc2d04-4322-41bc-b084-d111fb12356e.png)



To make the model unsupervised you have to remove the labelled data completly and allow the model to operate on its own unlabelled data

To include reinforcement the pandas model will have to remove the expected outcomes and leave the inputs to include reinforcement



## What does it do?

Pandas allows the computer to predict a certain outcome for a certain variable with the use of predetermined variables however it can become more accurate with the use of more predetermined variables this is possible as it is a multiple regression model. Below is an image of an ideal cluster and the second is a image of a multiple regression they are both different.

![image](https://user-images.githubusercontent.com/99629727/156592255-ed217902-34e9-42bc-a210-01f38bd1712d.png)



the image above shows a data set about cars the the algorithm can already make a guess of the C02 produced by the car based just on the size of the engine however it can become more accurate with an increase in independent variables




## Example

```python
import pandas
from sklearn import linear_model

df = pandas.read_csv("cars.csv")

X = df[['Weight', 'Volume']]
y = df['CO2']

regr = linear_model.LinearRegression()
regr.fit(X, y)

#predict the CO2 emission of a car where the weight is 2300kg, and the volume is 1300cm3:
predictedCO2 = regr.predict([[2300, 1300]])

print(predictedCO2)
```


## Deep learning

The model I used uses deep learning which is a subfield of machine learning it is a learning technique that allows computers to make more human like decisions.
