# 📊 Exercícios de Probabilidade

Este repositório contém diversos exercícios resolvidos sobre Probabilidade utilizando Python e bibliotecas como `scipy.stats`, `numpy`, `matplotlib`, `seaborn` e `statistics`.

## 📁 Bibliotecas Utilizadas

```python
from scipy.stats import binom, nbinom, poisson, uniform
import numpy as np
import matplotlib.pyplot as plt
import seaborn as sns
import statistics as st
```

## 📌 Exercícios

### 🎲 Distribuições e Probabilidades com Tabelas

```python
# Construção de uma matriz
matriz = [
    [26,28,54],
    [18,15,33],
    [9,11,20],
    [10,10],
    [2,6,8],
    [55,70,125]
]
```

#### Qual a probabilidade de sortear um funcionário com idade entre 35 e menos de 55 anos?
```python
print("P(35->54) =", ((matriz[2][2] + matriz[3][1]) / matriz[5][2]))  # R = 6/25
```

#### Sabendo-se que o funcionário é do gênero feminino, qual a probabilidade de ela ter entre 25 e menos de 35 anos?
```python
print("P(25->34|F) =", matriz[1][0] / matriz[5][0])  # R = 0,33
```

#### Qual a probabilidade do funcionário ser do gênero masculino ou ter idade entre 25 e menos de 35 anos?
```python
print("P(M U 25->34) =", (matriz[5][1] / matriz[5][2]) + (matriz[1][2] / matriz[5][2]) - (matriz[1][1] / matriz[5][2]))  # R = 0,70
```

### ⚽ Probabilidade de Todos Errarem o Pênalti
```python
(1 - 2/3) * (1 - 4/5) * (1 - 7/10)  # R = 1/50
```

### 🔌 Probabilidade em Circuitos com Relés

Fórmula da probabilidade:
```
P = 2p² - p⁴
```

### 🖥️ Probabilidade Condicional com Clientes de uma Rede
```python
P_E = 0.20
P_Er_E = 0.08
P_Er = (0.10*0.01 + 0.15*0.02 + 0.15*0.005 + 0.40*0.02 + 0.20*0.08)
P_E_Er = (P_E * P_Er_E) / P_Er  # R = 0,5565
```

### 📈 Distribuição Binomial

#### A maioria dos 10 usuários da página p20 acessam a p21?
```python
print("P(>5):", 1 - binom.cdf(5,10,0.70))  # R = 0,8497
```

#### Probabilidade de rejeitar um lote com 20 notebooks se 4 ou mais forem defeituosos:
```python
print("P(>=4):", 1 - binom.cdf(3,20,0.01))  # R = 0,00004
```

### 🧮 Distribuição de Poisson

#### Menos de 3 consultas ao banco de dados no próximo minuto
```python
print("P(x<3):", poisson.cdf(2,3))  # R = 0,4232
```

#### Entre 2 e 4 blecautes em um ano, dado média de 1 por ano
```python
x_0 = poisson.pmf(0,1)
x_1 = poisson.pmf(1,1)
x_0_4 = poisson.cdf(4,1)
print(x_0_4 - x_0 - x_1)  # R = 0,260
```

## 👨‍🏫 Orientador

Prof. Ms. Felicien Gonçalves Vásquez
