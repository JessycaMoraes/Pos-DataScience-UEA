# 📊 Probability Exercises

This repository contains various solved exercises on Probability using Python and libraries such as `scipy.stats`, `numpy`, `matplotlib`, `seaborn`, and `statistics`.

## 📁 Libraries Used

```python
from scipy.stats import binom, nbinom, poisson, uniform
import numpy as np
import matplotlib.pyplot as plt
import seaborn as sns
import statistics as st
```

## 📌 Exercises

### 🎲 Distributions and Probabilities with Tables

```python
# Matrix construction
matrix = [
    [26,28,54],
    [18,15,33],
    [9,11,20],
    [10,10],
    [2,6,8],
    [55,70,125]
]
```

#### What is the probability of selecting an employee aged between 35 and 54?
```python
print("P(35->54) =", ((matrix[2][2] + matrix[3][1]) / matrix[5][2]))  # R = 6/25
```

#### Given that the employee is female, what is the probability she is aged between 25 and 34?
```python
print("P(25->34|F) =", matrix[1][0] / matrix[5][0])  # R = 0.33
```

#### What is the probability that the employee is male or aged between 25 and 34?
```python
print("P(M U 25->34) =", (matrix[5][1] / matrix[5][2]) + (matrix[1][2] / matrix[5][2]) - (matrix[1][1] / matrix[5][2]))  # R = 0.70
```

### ⚽ Probability That All Players Miss the Penalty
```python
(1 - 2/3) * (1 - 4/5) * (1 - 7/10)  # R = 1/50
```

### 🔌 Probability in Relay Circuits

Probability formula:
```
P = 2p² - p⁴
```

### 🖥️ Conditional Probability with Network Clients
```python
P_E = 0.20
P_Er_E = 0.08
P_Er = (0.10*0.01 + 0.15*0.02 + 0.15*0.005 + 0.40*0.02 + 0.20*0.08)
P_E_Er = (P_E * P_Er_E) / P_Er  # R = 0.5565
```

### 📈 Binomial Distribution

#### Do most of the 10 users of page p20 access p21?
```python
print("P(>5):", 1 - binom.cdf(5,10,0.70))  # R = 0.8497
```

#### Probability of rejecting a batch of 20 notebooks if 4 or more are defective:
```python
print("P(>=4):", 1 - binom.cdf(3,20,0.01))  # R = 0.00004
```

### 🧮 Poisson Distribution

#### Less than 3 database queries in the next minute
```python
print("P(x<3):", poisson.cdf(2,3))  # R = 0.4232
```

#### Between 2 and 4 blackouts in a year, given an average of 1 per year
```python
x_0 = poisson.pmf(0,1)
x_1 = poisson.pmf(1,1)
x_0_4 = poisson.cdf(4,1)
print(x_0_4 - x_0 - x_1)  # R = 0.260
```

## 👨‍🏫 Advisor

Prof. Ms. Felicien Gonçalves Vásquez
