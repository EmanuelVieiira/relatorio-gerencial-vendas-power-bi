# 📈 Relatório Gerencial de Vendas e Lucro — Power BI

> Dashboard interativo de vendas e lucro, desenvolvido como desafio prático do bootcamp **Analisando Dados com SQL, Analytics e Power BI**, da [DIO](https://www.dio.me/).
>
> O projeto tem **duas versões**: a **Versão 1** (relatório original das aulas) e a **Versão 2**, reformulada com foco em **experiência do usuário**.

## 📑 Índice

- [Versão 2 — Foco em experiência do usuário](#-versão-2--foco-em-experiência-do-usuário)
- [Versão 1 — Relatório original](#-versão-1--relatório-original)
- [Tecnologias utilizadas](#️-tecnologias-utilizadas)
- [Fonte dos dados](#️-fonte-dos-dados)
- [Arquivos neste repositório](#-arquivos-neste-repositório)
- [Como abrir o projeto](#️-como-abrir-o-projeto)
- [Objetivo](#-objetivo)

---

## ✨ Versão 2 — Foco em experiência do usuário

A segunda versão reformula o relatório pensando em **como a pessoa lê e navega** pelo dashboard. O conteúdo e os gráficos principais foram mantidos, mas o layout, as cores e a navegação foram redesenhados, e foi criada uma terceira página de detalhamento.

### 🖼️ Prévia

#### Página 1 – Sales Report

![Sales Report](Versao-2/Sales%20Report.png)

#### Página 2 – Profit Report

![Profit Report](Versao-2/Profit%20Report.png)

#### Página 3 – Sales Detail

![Sales Detail](Versao-2/Sales%20Detail.png)

### 🎨 Decisões de design

| Princípio | Como foi aplicado |
|---|---|
| **Posicionamento** | Título no canto superior esquerdo, indicadores principais logo abaixo e filtros em um local fixo (canto superior direito) em todas as páginas. |
| **Leitura da esquerda para a direita** | A coluna da esquerda traz o contexto rápido (indicadores, botões de visão e gráfico por produto). O gráfico principal fica à direita, onde o olhar termina. |
| **Proporção áurea** | A página é dividida em cerca de **38% (esquerda) e 62% (direita)**, proporção próxima de 1 : 1,618. |
| **Contraste** | Fundo azul marinho com texto claro. A cor de destaque aparece só no que importa: botão da página atual, maior valor e valor principal. |
| **Segmentação dos dados** | Filtro de data com botão de limpar, botões de visão (Segmento/Produto e Países/Produto) e filtro por ano. |
| **Consistência** | Mesmo menu, mesma posição do título, mesmos cantos arredondados e mesma paleta nas três páginas. |

### 🌈 Paleta de cores

| Uso | Cor | Código |
|---|---|---|
| Fundo da página | Azul marinho | `#0B1F3A` |
| Cartões e visuais | Azul escuro | `#12305A` |
| Barras e séries secundárias | Azul médio | `#3F6FB5` |
| Cabeçalhos | Azul | `#1E4E8C` |
| Destaque | Âmbar | `#F5A623` |
| Texto | Branco gelo | `#F4F6FA` |
| Texto secundário | Cinza azulado | `#8A94A6` |

### 🧭 Navegação

- **Menu lateral** com os botões **Sales**, **Profit** e **Detail**, presente em todas as páginas.
- Cada botão tem três estados: **padrão**, **ao focalizar (hover)** e **selecionado**. O botão da página atual fica em destaque.
- **Seta** na parte inferior do menu para avançar ou voltar entre as páginas.
- **Botões de visão** que alternam o gráfico exibido, usando **marcadores (bookmarks)**.

### 🚀 Funcionalidades por página

#### 1. Sales Report

Visão geral das vendas:

- Indicadores: **Sum of Sales** e **Sum of Units Sold**
- **Filtro de período** com botão para limpar
- Botões **Visão Segmento / Visão Produto**, que alternam o gráfico de vendas por segmento ou por produto
- Gráfico de área **Sales by Period** (vendas ao longo dos meses)
- **Matriz** de vendas por ano, trimestre e segmento

#### 2. Profit Report

Análise do lucro:

- Indicadores: **Sum of Profit** e **Sum of Discounts**
- Botões **Visão Países / Visão Produto**, que alternam o gráfico de lucro por país ou por produto
- Gráfico de cascata (waterfall) com o **lucro por trimestre**
- Treemap do **lucro por segmento**
- Filtro por **ano** (2013 e 2014) e filtro de data

#### 3. Sales Detail

Detalhamento das vendas ao longo do tempo:

- Gráfico de área com **Sales e Profit por mês**
- **Matriz** com vendas por trimestre e ano
- Gráfico de **colunas e linha**: colunas de **Sum of Sales** e linha de **Sum of Gross Sales**, ordenadas do menor para o maior, com degradê de cor até o mês de maior venda

---

## 🧱 Versão 1 — Relatório original

Primeira versão do relatório, feita seguindo as aulas do bootcamp.

### 🖼️ Prévia

#### Página 1 – Sales Report

<img width="1118" height="622" alt="Sales Report" src="https://github.com/user-attachments/assets/31f54a6a-a21c-4203-9dc2-f9f210356294" />

#### Alternância entre visualizações

<img width="1118" height="622" alt="Pie Chart / Bar Chart" src="https://github.com/user-attachments/assets/63cf1827-d0b5-4faa-b087-6123bb4eccb9" />

#### Página 2 – Report de Lucro Detalhado

<img width="1118" height="622" alt="Report de Lucro Detalhado" src="https://github.com/user-attachments/assets/d06ad0be-c85f-418f-9608-23761fd1df13" />

### 🚀 Funcionalidades

#### 1. Sales Report

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

#### 2. Report de Lucro Detalhado

Página destinada a uma análise mais aprofundada do lucro, explorando os resultados por diferentes dimensões:

- Lucro por produto, segmento, trimestre e país
- Análise hierárquica do lucro por ano e país
- Filtros por ano e país

Usa **gráfico de radar, treemap, gráfico de cascata (waterfall) e árvore de decomposição**, além de um **botão de voltar** para retornar ao Sales Report.

---

## 🛠️ Tecnologias utilizadas

![Power BI](https://img.shields.io/badge/Power_BI-F2C811?style=flat&logo=powerbi&logoColor=black)

- **Power BI Desktop** — modelagem de dados, visualizações e navegação interativa entre páginas
- **Campos calculados e agregações nativas** — totais, evolução mensal e lucro por dimensão usando os recursos prontos do Power BI
- **Marcadores (bookmarks) e botões** — alternância entre visualizações e menu de navegação com estados de hover e seleção
- **Formas e temas personalizados** — fundo com cantos arredondados e paleta de cores consistente

## 🗂️ Fonte dos dados

Os dados utilizados foram disponibilizados pela expert no repositório original do curso:

🔗 https://github.com/julianazanelatto/power_bi_analyst

## 📎 Arquivos neste repositório

| Arquivo | Descrição |
|---|---|
| `Versao-2/Relatorio_v2.pbix` | **Versão 2** do relatório, com foco em experiência do usuário |
| `Versao-2/Sales Report.png` | Captura da página 1 da Versão 2 |
| `Versao-2/Profit Report.png` | Captura da página 2 da Versão 2 |
| `Versao-2/Sales Detail.png` | Captura da página 3 da Versão 2 |
| `Formação_Power_BI.pbit` | Arquivo original do projeto Power BI (template, Versão 1) |
| `Formação_Power_BI.pdf` | Exportação em PDF do relatório da Versão 1 |

## ▶️ Como abrir o projeto

1. Instale o [Power BI Desktop](https://www.microsoft.com/pt-br/power-platform/products/power-bi/downloads) (gratuito).
2. Para a **Versão 2**, baixe o arquivo `Versao-2/Relatorio_v2.pbix` e abra no Power BI Desktop.
3. Para a **Versão 1**, baixe o arquivo `Formação_Power_BI.pbit`. Como é um template (.pbit), ele pode pedir para reconectar a fonte de dados original (veja o link na seção acima).

> Não tem o Power BI instalado? Consulte as imagens da Versão 2 acima ou o `Formação_Power_BI.pdf` para ver o relatório em formato estático.

## 🎯 Objetivo

Projeto desenvolvido para praticar modelagem de dados e construção de dashboards interativos no Power BI, incluindo navegação entre páginas e alternância dinâmica entre tipos de visualização. Na Versão 2, o foco foi aplicar princípios de **design e experiência do usuário** (posicionamento, contraste, proporção áurea, segmentação e navegação) a um relatório já existente.
