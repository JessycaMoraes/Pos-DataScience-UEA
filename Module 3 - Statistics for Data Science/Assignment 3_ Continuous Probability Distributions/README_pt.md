# Exercícios de Distribuições de Probabilidade Contínua

## 📘 Descrição

Este repositório contém diversos exercícios envolvendo distribuições de probabilidade contínua utilizando bibliotecas como `scipy`, `numpy`, `matplotlib`, `seaborn` e `statistics`.

## 📚 Bibliotecas Utilizadas

```python
from scipy.stats import binom, nbinom, poisson, uniform, expon, norm
import numpy as np
import matplotlib.pyplot as plt
import seaborn as sns
import statistics as st
from scipy import stats
```

## 🧪 Exercícios

### 1. Distribuição Exponencial - Tempo de vida do transístor

Qual a probabilidade de um transístor durar entre 300 e 1000 horas?

```python
expon.cdf(1000, scale=500) - expon.cdf(300, scale=500)
# Resultado: 0.4135
```

### 2. Distribuição Normal - Notas de uma prova

Qual a probabilidade de um aluno tirar entre 7,0 e 8,0 pontos?

```python
norm.cdf(8, 6, 4) - norm.cdf(7, 6, 4)
# Resultado: 0.0928
```

### 3. Normal - 5% das garrafas abaixo de 1000 cm³

```python
norm.ppf(0.05, 1000, 10)
# Resultado: 983.6
```

### 4. Geração de Números Aleatórios - Distribuição Uniforme

```python
aleatorios = random.uniform(0, 1, size=100)
st.mean(aleatorios)           # Média ≈ 0.5591
st.pvariance(aleatorios)      # Variância ≈ 0.0808
```

Esperado: Média ≈ 1/2, Variância ≈ 1/12

### 5. Tamanho da amostra com erro amostral de 2%

```python
n = (norm.ppf(0.975)**2)*0.9*0.1/(0.02**2)
math.ceil(n)
# Resultado: 865
```

### 6. Intervalo de Confiança (IC) para proporção de sucessos

```python
inf, sup = prop.proportion_confint(80, 400, alpha=0.05, method='normal')
# Resultado: IC95%(16%, 24%)
```

### 7. IC para média populacional com desvio padrão conhecido

```python
inf, sup = norm.interval(0.99, loc=800, scale=100/np.sqrt(30))
# Resultado: IC99%(753.0; 847.0)
```

### 8. IC para média amostral com σ² = 1.96 e α = 5%

```python
x = [25.2, 26.0, 26.4, 27.1, 28.2, 28.4]
media = st.mean(x)
inf, sup = norm.interval(0.95, loc=media, scale=1.4/np.sqrt(6))
# Resultado: IC95%(25.76 ; 28.00)
```

## 👨‍🏫 Orientador

Prof. Ms. Felicien Gonçalves Vásquez
