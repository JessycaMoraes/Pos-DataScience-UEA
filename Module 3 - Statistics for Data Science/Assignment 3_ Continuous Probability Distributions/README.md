# Continuous Probability Distributions Exercises

## 📘 Description

This repository contains several exercises involving continuous probability distributions using libraries such as `scipy`, `numpy`, `matplotlib`, `seaborn`, and `statistics`.

## 📚 Libraries Used

```python
from scipy.stats import binom, nbinom, poisson, uniform, expon, norm
import numpy as np
import matplotlib.pyplot as plt
import seaborn as sns
import statistics as st
from scipy import stats
```

## 🧪 Exercises

### 1. Exponential Distribution – Transistor Lifetime

What is the probability that a transistor lasts between 300 and 1000 hours?

```python
expon.cdf(1000, scale=500) - expon.cdf(300, scale=500)
# Result: 0.4135
```

### 2. Normal Distribution – Test Scores

What is the probability that a student scores between 7.0 and 8.0?

```python
norm.cdf(8, 6, 4) - norm.cdf(7, 6, 4)
# Result: 0.0928
```

### 3. Normal – 5% of bottles under 1000 cm³

```python
norm.ppf(0.05, 1000, 10)
# Result: 983.6
```

### 4. Random Number Generation – Uniform Distribution

```python
aleatorios = random.uniform(0, 1, size=100)
st.mean(aleatorios)           # Mean ≈ 0.5591
st.pvariance(aleatorios)      # Variance ≈ 0.0808
```

Expected: Mean ≈ 1/2, Variance ≈ 1/12

### 5. Sample size for 2% error margin

```python
n = (norm.ppf(0.975)**2)*0.9*0.1/(0.02**2)
math.ceil(n)
# Result: 865
```

### 6. Confidence Interval (CI) for success proportion

```python
inf, sup = prop.proportion_confint(80, 400, alpha=0.05, method='normal')
# Result: CI95%(16%, 24%)
```

### 7. CI for population mean with known standard deviation

```python
inf, sup = norm.interval(0.99, loc=800, scale=100/np.sqrt(30))
# Result: CI99%(753.0; 847.0)
```

### 8. CI for sample mean with σ² = 1.96 and α = 5%

```python
x = [25.2, 26.0, 26.4, 27.1, 28.2, 28.4]
media = st.mean(x)
inf, sup = norm.interval(0.95, loc=media, scale=1.4/np.sqrt(6))
# Result: CI95%(25.76 ; 28.00)
```

## 👨‍🏫 Advisor

Prof. Ms. Felicien Gonçalves Vásquez
