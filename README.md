# 📊 Análise do Mercado de Dados no Brasil — Diversidade & Salários

![Status](https://img.shields.io/badge/Status-Em%20Desenvolvimento-yellow?style=for-the-badge)
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)
![Matplotlib](https://img.shields.io/badge/Matplotlib-11557c?style=for-the-badge&logo=python&logoColor=white)
![Seaborn](https://img.shields.io/badge/Seaborn-4C72B0?style=for-the-badge&logo=python&logoColor=white)
![Plotly](https://img.shields.io/badge/Plotly-3F4F75?style=for-the-badge&logo=plotly&logoColor=white)

> Projeto desenvolvido durante o curso **"Análise de Dados com Python — Meus Primeiros Passos"** da **Programaria**, comunidade voltada para mulheres na tecnologia. Análise exploratória dos dados da pesquisa **State of Data Brazil 2022** (Datahackers), com foco em diversidade de gênero, raça e desigualdade salarial no mercado de TI brasileiro.

---

## 🧩 Contexto

A pesquisa **State of Data Brazil** é realizada anualmente pela comunidade Datahackers e é uma das principais fontes de informação sobre o mercado de trabalho em dados no Brasil. A edição de 2022 coletou dados sobre salários, nível de escolaridade, gênero, raça, cargo, ferramentas utilizadas e muito mais.

Este projeto usa esses dados reais para responder perguntas como:

- 💰 Existe diferença salarial entre homens e mulheres na área de dados?
- 🎓 O nível de escolaridade influencia o salário?
- 🌍 A raça/etnia impacta a representatividade nos cargos de liderança?
- 📈 Qual a relação entre idade e salário?
- 👔 Quem são os gestores — e quem não é?

---

## 🎯 Objetivos

- Praticar análise exploratória de dados (EDA) com Python e Pandas
- Aplicar técnicas de limpeza e tratamento de dados reais
- Desenvolver visualizações claras e informativas
- Extrair insights sobre diversidade e desigualdade no mercado de TI

---

## 🔬 O que foi analisado

### 🧹 Tratamento de Dados
- Identificação e tratamento de valores nulos com estratégias diferenciadas por coluna
- Substituição de nulos em `IDADE` pela média da faixa etária correspondente
- Substituição de nulos em `SALARIO` pela mediana (mais robusta a outliers)
- Padronização da coluna `GENERO` (valores não informados → "Prefiro não informar")

### 📐 Estatística Descritiva
- Média, mediana, moda e desvio padrão por grupo
- Comparação salarial entre gêneros
- Análise de distribuição por faixa etária e geração

### 🔎 Detecção e Tratamento de Outliers
- Identificação via desvio padrão (limite: 3σ)
- Cálculo de IQR (Intervalo Interquartil) e limites do boxplot
- Substituição de outliers pela média da faixa salarial correspondente

### 🛠️ Feature Engineering
- Criação da coluna `GERACAO` a partir da idade (Geração X, Millennial, Geração Z)
- Criação da coluna `ETNIA_CLASS` agrupando raça/etnia em categorias analíticas
- Criação da coluna `NOVO_NIVEL` diferenciando pessoas gestoras dos demais níveis

### 📊 Correlação
- Correlação de Pearson entre `IDADE` e `SALARIO`
- Coeficiente de Cramér para variáveis categóricas (raça × nível de carreira)
- Tabelas cruzadas para análise de representatividade

### 📈 Visualizações
- Gráficos de barras com **Matplotlib** e **Seaborn**
- Gráficos de linha interativos com **Plotly**
- Scatter plot de dispersão salarial por idade
- Boxplot para identificação de outliers
- Mapa de calor de correlações

---

## 🛠️ Tecnologias Utilizadas

| Biblioteca | Uso |
|---|---|
| `Pandas` | Manipulação e análise de dados |
| `NumPy` | Operações numéricas e estatística |
| `Matplotlib` | Visualizações estáticas |
| `Seaborn` | Visualizações estatísticas |
| `Plotly` | Visualizações interativas |
| `SciPy` | Estatística avançada (intervalo de confiança, Cramér) |

---

## 📁 Estrutura do Repositório

```
analise-mercado-dados-brasil/
│
└── Uso_da_biblioteca_Pandas_em_Py_PROGRAMARIA.ipynb   # Notebook principal
```

---

## ▶️ Como executar

```bash
# Clone o repositório
git clone https://github.com/anna-kelly/analise-mercado-dados-brasil.git

# Acesse a pasta
cd analise-mercado-dados-brasil
```

Abra o notebook no **Google Colab** ou **Jupyter Notebook**.

> ⚠️ Os dados utilizados são da pesquisa **State of Data Brazil 2022** (Datahackers). O arquivo de dados não está incluso no repositório por questões de licenciamento — acesse em [datahackers.com.br](https://datahackers.com.br).

---

## 💡 Alguns Insights Encontrados

> *(Em construção — sendo atualizado conforme o curso avança)*

- 👩 Mulheres representam uma parcela significativamente menor dos cargos de gestão
- 💰 A diferença salarial entre gêneros é observável mesmo controlando por nível de carreira
- 📉 A correlação entre idade e salário existe, mas é mais fraca do que o esperado
- 🎓 O nível de escolaridade tem impacto relevante na faixa salarial

---

## 🗺️ Próximos Passos

```
✅ Tratamento de dados nulos
✅ Estatística descritiva por grupo
✅ Detecção e tratamento de outliers
✅ Feature Engineering
✅ Correlação entre variáveis
✅ Visualizações com Matplotlib, Seaborn e Plotly

🔄 Em andamento:
   → Análise aprofundada de diversidade de gênero e raça
   → Dashboard interativo com os principais insights
   → Conclusões e recomendações finais
```

---

## 🏫 Contexto do Curso

| | |
|---|---|
| **Curso** | Análise de Dados com Python — Meus Primeiros Passos |
| **Instituição** | Programaria |
| **Foco** | Mulheres na tecnologia |
| **Duração** | 60 horas |
| **Ano** | 2026 |
| **Ambiente** | Google Colab |

---

## 👩‍💻 Autora

**Anna Kelly Sousa** — Ex-Gerente Geral Bancária em transição para Dados

Como mulher em transição de carreira para tecnologia, este projeto tem um significado especial: analisar dados sobre o próprio mercado que estou ingressando, com foco em representatividade e equidade.

🔗 [GitHub](https://github.com/anna-kelly) · [LinkedIn](https://linkedin.com/in/anna-kelly-sousa-084a152b5)
