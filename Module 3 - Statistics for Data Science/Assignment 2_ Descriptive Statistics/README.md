# 📊 Statistical Analysis of Football Salaries

This project uses **Python** and libraries such as `pandas`, `numpy`, `seaborn`, `scipy`, and `statistics` to perform statistical analysis of player salaries from **PSG** and **Real Madrid**.

## 📁 Data Structure

The datasets were manually created as follows:

### 🟦 PSG

| Player        | Salary |
|---------------|--------|
| Neymar        | 37     |
| Mbappé        | 23     |
| Thiago Silva  | 18     |
| Cavani        | 16     |
| Marquinhos    | 14     |
| Verratti      | 14     |
| Di María      | 13     |
| Navas         | 12     |
| Icardi        | 10     |
| Paredes       | 9      |

### ⚪ Real Madrid

| Player           | Salary |
|------------------|--------|
| Hazard           | 15     |
| Gareth Bale      | 15     |
| Sergio Ramos     | 12     |
| Tony Kroos       | 12     |
| Luka Modric      | 11     |
| Marcelo          | 10     |
| Benzema          | 9      |
| James Rodríguez  | 9      |
| Courtois         | 9      |
| Vinícius Jr      | 7      |

---

## 📈 Statistical Analysis

### ✅ Salary Skewness

- **PSG**: Positively skewed (Skewness: 1.96)
- **Real**: Mode < Median < Mean

### 📏 Mean, Median, and Mode

#### PSG:
- Mean: 16.6
- Median: 14.0
- Mode: 14 (most frequent)

#### Real:
- Mean: 10.9
- Median: 10.5
- Mode: 9 (most frequent)

### 📊 Visualization

Distribution plots and boxplots were used to identify outliers and shape.

### 📉 Variability

#### Standard Deviation:
- PSG: 8.22
- Real: 2.64

#### Coefficient of Variation (CV):
- PSG: 49.53%
- Real: 24.25%

📌 **Conclusion**: Real Madrid has both lower average salary and lower variability.

---

## 🧮 Interquartile Range (Real)

- Q1: 9.0
- Q3: 12.0
- IQR: **3.0**

---

## 🧠 Outliers

Based on **boxplots**, outliers were only found in the PSG salaries.

---

## ⚽ Goal Performance

Real Madrid's goal distribution:

```python
X = {(0,5), (1,3), (2,4), (3,3), (4,2), (5,2), (7,1)}
```

- Mean: 2.25
- Median: 2.0
- Mode: 0

✔️ Conclusion: Mode < Median < Mean

---

## 👨‍🏫 Advisor

Prof. Ms. Felicien Gonçalves Vásquez
