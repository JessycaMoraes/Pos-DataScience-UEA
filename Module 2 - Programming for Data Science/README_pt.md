# 📊 Análise Exploratória de Dúvidas sobre a COVID-19 nas Redes Sociais

## 🧠 Visão Geral

Durante o surto da COVID-19, a América Latina foi uma das regiões mais afetadas, com o **Brasil apresentando o maior número de casos**. 

Redes sociais como **Twitter, Facebook e Instagram** se tornaram fontes fundamentais para observar comportamentos, sentimentos e **dúvidas da população** em tempo real. Este projeto tem como objetivo utilizar essas informações para **auxiliar gestores públicos** a tomarem decisões mais informadas durante a pandemia.

Nosso foco está na análise de dados do **Twitter**, uma plataforma de alto volume e troca rápida de informações, similar ao **Weibo**, amplamente utilizado na China. 

> 🎯 A proposta central é realizar uma **análise exploratória das dúvidas postadas por usuários do Twitter relacionadas à COVID-19**, extraindo padrões, variações temporais e geográficas.

---

## 🎯 Objetivos

- 📌 Apresentar e explorar amostras dos dados coletados;
- 🤖 Extrair e classificar perguntas (dúvidas) dos tweets;
- 🧾 Gerar um dataset chamado `duvidasDb` com as perguntas extraídas; 
- 📊 Analisar as perguntas sob diferentes perspectivas:

### 🔍 Visão Geral dos Dados
- Resumo (sumário) com as estatísticas dos dados originais, ou seja, sem
qualquer pré-processamento;
- As estatísticas podem ser apresentadas através de tabelas e/ou gráficos.

### 📚 Classificação das Perguntas
- Dúvidas relacionadas a:
  - Doenças - Quando a pergunta é relativa à doença. Deve-se observar que a doença é identificada por vários nomes. Exemplo: coronavírus, corona, COVID-19, etc.
  - Medicamentos - Quando a pergunta é sobre o uso de determinado medicamento no tratamento da doença.
  - Organizações - Quando a pergunta é relativa a uma determinada entidade ou organização. Emissora de TV, Ministério da Saúde ou empresas são exemplos de organizações.
  - Pessoas - Quando a pergunta é sobre determinada pessoa. Por exemplo, a pergunta pode ser sobre a atuação que determinado político ou pessoa famosa teve durante esse período de
pandemia.

### ⏳ Visão Temporal
- Pode-se considerar o intervalo temporal de dias, semanas ou meses;
- Fazer uma análise temporal das perguntas que formam o dataset. Exemplo:
  - Houve aumento no número de perguntas ao longo do tempo?
  - O perfil das perguntas mudou com o tempo?

### 🗺️ Visão Geográfica
- Deve-se fazer uma análise geográfica (espacial) das perguntas que formam o dataset;
- Exemplo de análise geográfica:
  - a) os usuários de regiões diferentes fazem perguntas com diferentes focos?
- Essa análise ainda pode ser realizada em diversos níveis de área (cidade, estado ou região);
- Apresentar a distribuição das dúvidas dos usuários por região;
- Deverá fazer uma análise dessa distribuição. Exemplo:
  - Apresentar as razões (ou hipóteses) da ocorrência dessa distribuição.

---

## 🗂️ Dataset

A base de dados será fornecida pelo professor e estará disponível em:

🔗 [tiagodemelo.info](http://tiagodemelo.info)

---

## 🧰 Tecnologias Utilizadas

- 🐍 Python 3
- 🧮 Pandas, NumPy
- 📈 Matplotlib, Seaborn

---

## 👥 Equipe

- Jessyca Moraes  
- Gian Silva

👨‍🏫 **Orientador**: Prof. Tiago de Melo - [tmelo@uea.edu.br](mailto:tmelo@uea.edu.br)

---

> 🧪 Em caso de dúvidas ou contribuições, sinta-se à vontade para abrir uma issue ou entrar em contato.
