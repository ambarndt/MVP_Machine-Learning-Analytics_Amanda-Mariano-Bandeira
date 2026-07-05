# MVP_Machine-Learning-Analytics_Amanda-Mariano-Bandeira
Repositório criado para hospedagem do MVP de Machine Learning, da pós-graduação da PUC-Rio.  
Julho/2026

**Amanda Mariano Bandeira  
Curso: Data Science and Analytics**

##Contexto

A previsão de produção de óleo é uma das atividades mais importantes na gestão de campos de petróleo. Compreender o declínio natural desses campos permite uma gestão mais eficiente e melhor planejamento de investimentos. Este projeto de MVP aplica técnicas de Machine Learning para prever a produção mensal de óleo do campo de Polvo, na bacia de Campos, atualmente operado pela PRIO, utilizando exclusivamente dados públicos de produção fornecidos pela ANP.

##Objetivo

Construir e avaliar modelos de regressão para prever a produção mensal de óleo de um campo, comparando com modelos mais robustos e discutindo os resultados obtidos.

##Dataset

Fonte: ANP  
Campo: Polvo  
Operador: PRIO  
Granularidade: mensal, a nível de campo  
Variável-alvo: produção de óleo (bbl/d)

##Abordagem

* Regressão com features temporais
* Divisão temporal sem embaralhamento
* Prevenção de vazamento de dados

##Resultados

| Modelo | Métrica principal (MAE) | RMSE | R2 |  
| Baseline | 4904.50 | 5341.15 | -22.8853 |  
| Random Forest | 967.18 | 1211.66 | -0.2292 |  
| Gradient Boosting | 664.51 | 973.46 | 0.2066 |  
| Gradient Boosting otimizado | 769.5 | 1034.66 | 0.1037 |

**Modelo escolhido:** Gradient Boosting (sem otimização). Apresentou o menor MAE e tem R2 positivo. Superou o baseline em 86%, com tempo de treino foi rápido.


