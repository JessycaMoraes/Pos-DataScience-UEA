# Metodologia para o Trabalho Final de Estatística para Ciência de Dados

## Objetivo

Definir um tema e realizar um levantamento amostral atendendo os procedimentos a seguir.

## Procedimentos Gerais

- Serão criados grupos com no mínimo **3** e no máximo **5 alunos**;
- Cada grupo terá um representante que será responsável por postar o nome dos componentes no mural do Classroom, que será disponibilizado para postagem do trabalho;
- A avaliação vale de **zero a sete pontos**;
- A definição do tema e dos objetivos ficará na responsabilidade de cada grupo;
- O **data frame** terá que conter no mínimo **cinco campos** e **25 linhas**, sendo pelo menos **dois campos numéricos**;
- Todas as análises deverão ser realizadas no **Python** e apresentadas durante a aula do dia **14/11**;
- Os dados, juntamente com o notebook com os scripts, precisarão ser postados **antes da apresentação da primeira equipe**, que deve durar em média **10 minutos**;
- A ordem de apresentação dos grupos será realizada por meio de **sorteio**.

## Análises que deverão ser realizadas

a) (Vale **1,0 ponto**) Construir tabelas e gráficos apropriados para cada variável do data frame;  
b) (Vale **1,0 ponto**) Calcular a **média**, **mediana**, **moda**, **desvio-padrão**, **coeficiente de variação** e **simetria** das variáveis quantitativas;  
c) (Vale **1,0 ponto**) Analisar a **normalidade** dos dados numéricos e se existe a presença de **outliers**;  
d) (Vale **1,0 ponto**) Comparar as variáveis quantitativas e descrever qual é mais **homogênea**;  
e) (Vale **1,0 ponto**) Calcular os respectivos **Intervalos de Confiança** ao nível de **95%** para cada campo do data frame;  
f) (Vale **1,0 ponto**) Comparar a média de um campo numérico em relação a um campo categórico e responder se existe **diferença estatística ao nível de 5% de significância**;  
g) (Vale **1,0 ponto**) Realizar um cruzamento de dois campos categóricos e responder se existe **diferença estatística ao nível de 5% de significância**.

## Dataset

O dataset consiste de dados estatísticos oficiais dos **11.538 atletas** que participaram dos **Jogos Olímpicos de 2016 no Rio de Janeiro**. Ele inclui:

- Nome  
- Nacionalidade (em código de 3 dígitos)  
- Gênero  
- Data de nascimento  
- Altura (em metros)  
- Peso (em kg)  
- Modalidade esportiva  
- Quantidade de medalhas de ouro, prata e/ou bronze  

**Fonte**: [Kaggle](https://www.google.com/url?q=https%3A%2F%2Fwww.kaggle.com%2Frio2016%2Folympic-games%2F)

### Para fim disciplinar:

- Adquirimos a **idade** de cada atleta (para agosto/2016) a partir de sua data de nascimento, gerando assim uma nova coluna `age`;  
- Excluímos as colunas `id`, `name` e `dob`.
