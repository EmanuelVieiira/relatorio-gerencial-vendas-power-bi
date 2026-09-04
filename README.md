# 📈 Relatório Gerencial de Vendas — Power BI

> Dashboard interativo de vendas e lucro, desenvolvido como desafio prático do bootcamp **Analisando Dados com SQL, Analytics e Power BI**, da [DIO](https://www.dio.me/).

## 🖼️ Prévia do relatório

### Página 1 – Sales Report

<img width="1118" height="622" alt="Sales Report" src="https://github.com/user-attachments/assets/31f54a6a-a21c-4203-9dc2-f9f210356294" />

### Alternância entre visualizações

<img width="1118" height="622" alt="Pie Chart / Bar Chart" src="https://github.com/user-attachments/assets/63cf1827-d0b5-4faa-b087-6123bb4eccb9" />

### Página 2 – Report de Lucro Detalhado

<img width="1118" height="622" alt="Report de Lucro Detalhado" src="https://github.com/user-attachments/assets/d06ad0be-c85f-418f-9608-23761fd1df13" />

## 🚀 Funcionalidades

### 1. Sales Report

Dashboard destinado à análise geral das vendas, apresentando indicadores e visualizações sobre o desempenho comercial:

- Total de Vendas
- Total de Unidades Vendidas
- Total de Descontos
- Total de COGS
- Evolução das vendas por mês
- Vendas por segmento, produto e país

A página possui um **filtro de período** e **botões de navegação entre tipos de visualização**:

- **Pie Chart / Bar Chart** — alterna entre gráfico de pizza e de barras para vendas por segmento.
- **Map Chart / Treemap** — alterna entre mapa e treemap para distribuição de vendas por país.

### 2. Report de Lucro Detalhado

Página destinada a uma análise mais aprofundada do lucro, explorando os resultados por diferentes dimensões:

- Lucro por produto, segmento, trimestre e país
- Análise hierárquica do lucro por ano e país
- Filtros por ano e país

Usa **gráfico de radar, treemap, gráfico de cascata (waterfall) e árvore de decomposição**, além de um **botão de voltar** para retornar ao Sales Report.

## 🛠️ Tecnologias utilizadas

![Power BI](https://img.shields.io/badge/Power_BI-F2C811?style=flat&logo=powerbi&logoColor=black)

- **Power BI Desktop** — modelagem de dados, visualizações e navegação interativa entre páginas
- **Campos calculados e agregações nativas** — totais, evolução mensal e lucro por dimensão usando os recursos prontos do Power BI

## 🗂️ Fonte dos dados

Os dados utilizados foram disponibilizados pela expert no repositório original do curso:

🔗 https://github.com/julianazanelatto/power_bi_analyst

## 📎 Arquivos neste repositório

| Arquivo | Descrição |
|---|---|
| `Formação_Power_BI.pbit` | Arquivo original do projeto Power BI (template) |
| `Formação_Power_BI.pdf` | Exportação em PDF do relatório completo |

## ▶️ Como abrir o projeto

1. Instale o [Power BI Desktop](https://www.microsoft.com/pt-br/power-platform/products/power-bi/downloads) (gratuito).
2. Baixe o arquivo `Formação_Power_BI.pbit` deste repositório.
3. Abra o arquivo no Power BI Desktop — como é um template (.pbit), ele pode pedir para reconectar a fonte de dados original (veja o link na seção acima).

> Não tem o Power BI instalado? Basta consultar o `Formação_Power_BI.pdf` para ver o relatório completo em formato estático.

## 🎯 Objetivo

Projeto desenvolvido para praticar modelagem de dados e construção de dashboards interativos no Power BI, incluindo navegação entre páginas e alternância dinâmica entre tipos de visualização.
