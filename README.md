# 🏨 Limpeza e Tratamento de Dados de Reserva de Hotéis (Hotel Booking Data Cleaning)

![Python](https://img.shields.io/badge/Python-3.x-blue?style=for-the-badge&logo=python)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Cleaning-150458?style=for-the-badge&logo=pandas)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-F37626?style=for-the-badge&logo=jupyter)

## 📌 Visão Geral do Projeto
Este projeto tem como objetivo realizar o **tratamento, limpeza, padronização e validação de dados** de uma base bruta de reservas hoteleiras (*Hotel Booking Dataset*). 

Dados inconsistentes ou com valores ausentes podem comprometer relatórios financeiros e análises de cancelamento. Através deste pipeline em Python, a base de dados foi tratada e preparada para análises exploratórias.

---

## 🛠️ Tecnologias e Ferramentas Utilizadas
- **Linguagem:** Python 3.x
- **Bibliotecas Principais:** `pandas`, `numpy`
- **Ambiente de Desenvolvimento:** Jupyter Notebook / VS Code

---

## 🔍 Etapas do Processo de Limpeza (Data Cleaning Pipeline)

1. **Análise Exploratória Inicial e Identificação de Problemas:**
   - Verificação de tipos de dados (`dtypes`), valores nulos (`NaN`) e duplicados.
   - Identificação de discrepâncias em colunas categóricas e numéricas.

2. **Tratamento de Valores Ausentes (*Missing Values*):**
   - Imputação estratégica de dados (ex: substituição de nulos por valores padrão ou pela mediana/moda do contexto).
   - Remoção de registos sem informação crítica e irrecuperável.

3. **Padronização e Conversão de Tipos:**
   - Correção e conversão de colunas de datas (`datetime`).
   - Ajuste de colunas numéricas (ex: número de hóspedes, crianças, noites reservadas) para tipos inteiros adequados (`int64`).
   - Normalização de textos e categorias.

4. **Tratamento de Anomalias e Outliers:**
   - Filtro de registos inconsistentes (ex: reservas com 0 adultos, 0 crianças e 0 bebés).
   - Criação de novas colunas derivadas (*Feature Engineering*) para facilitar análises de negócio (ex: total de hóspedes, total de noites de estadia).
