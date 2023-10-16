## Project Title: Prediction using supervised ML

This project aims to predict the scores of students based on the number of hours they study per day using supervised machine learning techniques.

## Getting Started

### Prerequisites

To run this project, you need to have the following prerequisites installed:

- Python (version 3.0 or above)
- Jupyter Notebook or any other Python IDE
- Libraries: `numpy`, `pandas`, `matplotlib`, `scikit-learn`

### Dataset

The dataset used for this project can be found at the following link: [database](http://bit.ly/w-data)

Please download the dataset and save it in the same directory as the project files.

### Usage

1. Launch Jupyter Notebook or your preferred Python IDE.

2. Open the `TASK1.ipynb` file.

3. Run the notebook cell by cell to see the step-by-step process and results.

4. You will find the scatter plot visualization of the data, the training of the machine learning model, and the predictions based on the number of study hours.

### Code Explanation

The code in the `TASK1.ipynb` notebook follows the steps mentioned below:

1. Import necessary libraries:

```python
import numpy as np
import pandas as pd
from sklearn.linear_model import LinearRegression
import matplotlib.pyplot as plt
```

2. Load the dataset:

```python
df = pd.read_csv('http://bit.ly/w-data')
```

3. Visualize the data using a scatter plot:

```python
plt.scatter(data['Hours'], data['Scores'])
plt.xlabel('Hours Studied')
plt.ylabel('Scores')
plt.title('Hours Studied vs Scores')
plt.show()
```

4. Train the model using linear regression:

```python
reg = LinearRegression()
X= df[['Hours']].values
y= df['Scores'].values
reg.fit(X,y)
```

5. Predict the values using the trained model:

```python
result= reg.predict([[9.25]])
```

#### This code is successful for predicting the y scores of the students who studies x hours per day
