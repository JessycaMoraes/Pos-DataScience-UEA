# 📊 Análise Estatística de Salários no Futebol

Este projeto utiliza **Python** e bibliotecas como `pandas`, `numpy`, `seaborn`, `scipy` e `statistics` para realizar uma análise estatística dos salários dos jogadores dos clubes **PSG** e **Real Madrid**.

## 📁 Estrutura dos Dados

As bases foram criadas manualmente com os seguintes dados:

### 🟦 PSG

| Jogador       | Salário |
|---------------|---------|
| Neymar        | 37      |
| Mbappé        | 23      |
| Thiago Silva  | 18      |
| Cavani        | 16      |
| Marquinhos    | 14      |
| Verratti      | 14      |
| Di María      | 13      |
| Navas         | 12      |
| Icardi        | 10      |
| Paredes       | 9       |

### ⚪ Real Madrid

| Jogador           | Salário |
|-------------------|---------|
| Hazard            | 15      |
| Gareth Bale       | 15      |
| Sergio Ramos      | 12      |
| Tony Kroos        | 12      |
| Luka Modric       | 11      |
| Marcelo           | 10      |
| Benzema           | 9       |
| James Rodríguez   | 9       |
| Courtois          | 9       |
| Vinícius Jr       | 7       |

---

## 📈 Análises Estatísticas

### ✅ Simetria dos salários

- **PSG**: Assimétrica positiva (Coeficiente de Assimetria: 1.96)
- **Real**: Moda < Mediana < Média

### 📏 Média, Mediana e Moda

#### PSG:
- Média: 16.6
- Mediana: 14.0
- Moda: 14 (mais frequente)

#### Real:
- Média: 10.9
- Mediana: 10.5
- Moda: 9 (mais frequente)

### 📊 Visualização

Distribuições e boxplots foram usados para identificar outliers e a forma da distribuição dos salários.

### 📉 Variabilidade

#### Desvio-padrão:
- PSG: 8.22
- Real: 2.64

#### Coeficiente de Variação (CV):
- PSG: 49.53%
- Real: 24.25%

📌 **Conclusão**: O Real Madrid tem menor média e menor variabilidade salarial comparado ao PSG.

---

## 🧮 Amplitude Interquartil (Real)

- Q1: 9.0
- Q3: 12.0
- Amplitude Interquartil: **3.0**

---

## 🧠 Outliers

Através do **boxplot**, foi possível observar outliers apenas nos salários do PSG.

---

## ⚽ Desempenho de gols

Distribuição de gols do Real Madrid:

```python
X = {(0,5), (1,3), (2,4), (3,3), (4,2), (5,2), (7,1)}
```

- Média: 2.25
- Mediana: 2.0
- Moda: 0

✔️ Conclusão: Moda < Mediana < Média

---

## 👨‍🏫 Orientador

Prof. Ms. Felicien Gonçalves Vásquez
