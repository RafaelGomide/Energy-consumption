# Energy Consumption Prediction

Regressão supervisionada para previsão de consumo energético
em edificações residenciais, comerciais e industriais.

## Abordagem

- Geração de dataset sintético com relações lineares realistas
  entre área, ocupantes, aparelhos e temperatura
- Preprocessamento: conversão de variáveis categóricas
- Modelagem com XGBoost Regressor
- Otimização de hiperparâmetros via GridSearchCV (5-fold CV)
- Early stopping para controle de overfitting

## Resultados

| Modelo | RMSE |
|--------|------|
| XGBoost (default) | 543.55 |
| XGBoost (tuned) | 503.77 |

Melhora de ~7.3% com tuning de hiperparâmetros.

## Tecnologias

`Python` `pandas` `numpy` `XGBoost` `scikit-learn` `matplotlib` `seaborn`

## Como executar

```bash
git clone https://github.com/RafaelGomide/Energy-consumption
pip install pandas numpy xgboost scikit-learn matplotlib seaborn
jupyter notebook energy_consumption.ipynb
```

## Limitações

Dataset sintético criado para fins de estudo —
os coeficientes da relação consumo/variáveis foram definidos manualmente.
