# Projeto de Previsão de Vendas - Olist Dataset

![Python](https://img.shields.io/badge/Python-3.10-blue)
![Libraries](https://img.shields.io/badge/Libraries-Pandas%2C%20NumPy%2C%20Matplotlib%2C%20Seaborn%2C%20Scikit--learn-brightgreen)
![Status](https://img.shields.io/badge/Status-Completo-success)

## Objetivo
Prever a receita diária do e-commerce Olist, analisando padrões de vendas e fatores que influenciam a receita. O projeto também gera previsões para os próximos dias, permitindo planejamento de estoque, marketing e estratégias de vendas.

---

## Dataset

- Fonte: [Olist Brazilian E-Commerce](https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce)
- Período: 2016 a 2018
- Principais tabelas usadas: `orders`, `order_items`, `products`
- Colunas principais: preço, quantidade de pedidos, data da compra, categoria de produtos

> Os datasets originais não estão incluídos no repositório. É necessário baixá-los via KaggleHub para rodar o notebook completo.

---

## Metodologia

1. **Preparação de dados:** limpeza, conversão de datas, criação de features (dia da semana, mês, dia).  
2. **Análise exploratória:** visualizações de receita diária, por dia da semana e por mês; identificação de produtos e categorias mais lucrativas.  
3. **Modelagem preditiva:** Linear Regression, Random Forest e Gradient Boosting; avaliação via RMSE, MAE e R².  
4. **Previsão futura:** estimativa de receita para os próximos 7 dias.  
5. **Geração de insights:** crescimento médio mensal, dias/mês mais lucrativos, ticket médio, top produtos e categorias.

---

## Principais Resultados

- **Melhor modelo:** Linear Regression (R² = 0.88)  
- **Receita média diária:** R$ 22.064,36  
- **Dia com maior receita:** 2017-11-24  
- **Dia com menor receita:** 2016-12-23  
- **Crescimento médio mensal:** 48.790,24%  
- **Dia da semana mais lucrativo:** 1 (0=Segunda, 6=Domingo)  
- **Mês mais lucrativo:** 11  
- **Ticket médio por pedido:** R$ 137,75  
- **Número de dias com receita 30% abaixo da média:** 202  
- **Desvio padrão da receita diária:** 12.594,03  

### Top 5 Produtos por Quantidade Vendida

| Product ID | Quantidade |
|------------|------------|
| aca2eb7d00ea1a7b8ebd4e68314663af | 527 |
| 99a4788cb24856965c36a24e339b6058 | 488 |
| 422879e10f46682990de24d770e7f83d | 484 |
| 389d119b48cf3043d311335e499d9c6b | 392 |
| 368c6c730842d78016ad823897a372db | 388 |

### Top 5 Produtos por Receita

| Product ID | Receita (R$) |
|------------|--------------|
| bb50f2e236e5eea0100680137654686c | 63.885,00 |
| 6cdd53843498f92890544667809f1595 | 54.730,20 |
| d6160fb7873f184099d9bc95e30376af | 48.899,34 |
| d1c427060a0f73f6b889a5c7c61f2ac4 | 47.214,51 |
| 99a4788cb24856965c36a24e339b6058 | 43.025,56 |

### Top 5 Categorias por Receita

| Categoria | Receita (R$) |
|-----------|--------------|
| beleza_saude | 1.258.681,34 |
| relogios_presentes | 1.205.005,68 |
| cama_mesa_banho | 1.036.988,68 |
| esporte_lazer | 988.048,97 |
| informatica_acessorios | 911.954,32 |

---

## Previsão de Receita para os Próximos 7 Dias

| Data | Receita Prevista (R$) |
|------|-----------------------|
| 2018-09-04 | 20.915,55 |
| 2018-09-05 | 20.780,07 |
| 2018-09-06 | 20.644,60 |
| 2018-09-07 | 20.509,12 |
| 2018-09-08 | 20.373,64 |
| 2018-09-09 | 20.238,16 |
| 2018-09-10 | 20.879,74 |

> O gráfico de previsão mostra a tendência esperada, permitindo planejamento de estoque, marketing e estratégias de vendas.

---

## Conclusão

O modelo Linear Regression apresentou o melhor desempenho para previsão de receita diária. Observa-se crescimento médio mensal consistente, com maior faturamento em determinados dias da semana e meses do ano. Produtos e categorias mais lucrativos podem ser priorizados para ações de marketing e gestão de estoque. As vendas apresentam variação diária com desvio padrão de R$ 12.594,03, indicando estabilidade geral do negócio.

---

## Tecnologias e Bibliotecas Utilizadas

- Python 3
- Pandas, Numpy
- Matplotlib, Seaborn
- Scikit-learn (LinearRegression, RandomForestRegressor, GradientBoostingRegressor)
- KaggleHub (para download do dataset)
