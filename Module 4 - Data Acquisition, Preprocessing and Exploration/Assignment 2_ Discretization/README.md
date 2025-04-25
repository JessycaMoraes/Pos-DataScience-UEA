# 📊 Discretization Exercise

### 🎯 Goal

Perform data analysis and transformation on the `kc_house_data.csv` dataset using preprocessing, feature importance analysis, and dimensionality reduction techniques.

---

### 📝 Steps

1. **Select Columns**
   - Keep only:
     - `price`
     - `yr_built`
     - `yr_renovated`
     - `sqft_living`
     - `sqft_lot`
     - `sqft_lot15`
   - Target attribute (class): `condition`

2. **Attribute Discretization**
   - `condition`: 
     - Value **0** for bad conditions (between 1 and 3)
     - Value **1** for good conditions (greater than 3)
   - `yr_renovated`:
     - Value **0** if not renovated
     - Value **1** if renovated

3. **Feature Importance Analysis**
   - Use **three different methods** to determine attribute importance.
   - Compare the results.

4. **Data Normalization**
   - Normalize numerical attributes.
   - Repeat feature importance analysis with normalized data.
   - Compare with raw data results.

5. **Data Discretization**
   - Discretize numerical attributes.
   - Repeat feature importance analysis.
   - Compare with previous results.

6. **Dimensionality Reduction**
   - Apply techniques to reduce the final DataFrame dimensions.

7. **Export**
   - Store the final DataFrame in a new `.csv` file.

---

## 👨‍🏫 Advisor

Prof. Luis Cuevas Rodríguez, PhD
