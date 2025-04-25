# 📊 Exercício de Discretização

### 🎯 Objetivo

Realizar uma análise e transformação de dados a partir do dataset `kc_house_data.csv`, aplicando técnicas de pré-processamento, análise de importância dos atributos e redução de dimensionalidade.

---

### 📝 Etapas

1. **Selecionar colunas**
   - Manter apenas os atributos:
     - `price`
     - `yr_built`
     - `yr_renovated`
     - `sqft_living`
     - `sqft_lot`
     - `sqft_lot15`
   - Atributo alvo (classe): `condition`

2. **Discretização dos atributos**
   - `condition`: 
     - Valor **0** para condições ruins (entre 1 e 3)
     - Valor **1** para boas condições (maior que 3)
   - `yr_renovated`:
     - Valor **0** se não houve renovação
     - Valor **1** se houve renovação

3. **Análise de Importância dos Atributos**
   - Utilizar **três métodos distintos** para calcular a importância de cada atributo.
   - Comparar os resultados.

4. **Normalização dos dados**
   - Aplicar normalização nos atributos numéricos.
   - Repetir a análise de importância dos atributos com dados normalizados.
   - Comparar os resultados com os dados brutos.

5. **Discretização dos dados**
   - Discretizar os atributos numéricos.
   - Repetir a análise de importância com os dados discretizados.
   - Comparar os resultados.

6. **Redução de Dimensionalidade**
   - Aplicar técnicas para redução de dimensionalidade no DataFrame final.

7. **Exportação**
   - Armazenar o DataFrame final em um novo arquivo `.csv`.

---

## 👨‍🏫 Orientador

Prof. Luis Cuevas Rodríguez, PhD
