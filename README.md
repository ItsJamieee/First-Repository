# Machine learning

With this project I have decided to use Panda as my python library.

The guide I used for my project is linked [here](https://www.w3schools.com/python/python_ml_multiple_regression.asp)

## What model is this based on?

Linear regression is predicting the value of a dependent variable based on the independent variable.

Pandas uses multiple regression as its machine learning model, multiple regression is similar to linear regression however there is more than one independent value.

Multiple regression is a form of supervised learning which is when the algorithm is fed with labelled training data. The labbeled data has the outcome for the inputted data it uses the data to recognize patterns.

### Possible adaptation:



## What does it do?

Pandas allows the computer to predict a certain outcome for a certain variable with the use of predetermined variables however it can become more accurate with the use of more predetermined variables this is possible as it is a multiple regression model.

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



