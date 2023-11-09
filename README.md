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
import requests

def print_github_stats(ayebaishmo):
    url = f'https://api.github.com/users/{ayebaishmo}'
    response = requests.get(url)
    
    if response.status_code == 200:
        data = response.json()
        print(f"GitHub Stats for {username}:")
        print(f"Public Repositories: {data['public_repos']}")
        print(f"Followers: {data['followers']}")
        print(f"Following: {data['following']}")
        print(f"Bio: {data['bio']}")
    else:
        print(f"Failed to fetch GitHub stats. Status code: {response.status_code}")

# Replace 'your_username' with your actual GitHub username
print_github_stats('ayebaishmo')



