# Hello am Ayebazibwe Ishmael @ayebaishmo
[![Twitter Badge](https://img.shields.io/badge/-@ayebaishmo-1ca0f1?style=flat-square&labelColor=1ca0f1&logo=twitter&logoColor=white&link=https://twitter.com/ishmo256)](https://twitter.com/ishmo256)

```python
import pandas as pd
import numpy as np
from sklearn.model_selection import train_test_split
from sklearn.linear_model import LinearRegression
from sklearn.metrics import mean_squared_error

data = pd.read_csv("AI.csv")

X = data[['analyst', 'scientist']]
y = data['ML']

X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=0.2, random_state=42)

model = LinearRegression()

model.fit(X_train, y_train)
y_pred = model.predict(X_test)

mse = mean_squared_error(y_test, y_pred)
print("Mean Squared Error:", mse)


```
[![GitHub followers](https://img.shields.io/github/followers/?label=Followers&style=social)](https://github.com/ayebaishmo)
[![GitHub stars](https://img.shields.io/github/stars/your_username/your_repo?style=social)](https://github.com/ayebaishmo/ayebaishmo)
[![GitHub forks](https://img.shields.io/github/forks/your_username/your_repo?style=social)](https://github.com/ayebaishmo/ayebaishmo)




