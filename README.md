## Análise da base Airbnb - Rio de Janeiro

### a. Como foi a definição da sua estratégia de modelagem? 

A predição do preço foi escolhida pois essa é uma variável muito relevante.

### b. Como foi definida a função de custo utilizada? 

Como o preço não pode ser negativo, a distribuição gamma com minimação do desvio é adequada.

### c. Qual foi o critério utilizado na seleção do modelo final? 

Comparação de diversas métricas de erro incluindo desvio, MRAE e RMSE.

### d. Qual foi o critério utilizado para validação do modelo?

Foi realizada um validação cruzada 5-fold no modelo LGBM. O banco foi separado 60% para treino, 20% para validação dos modelos e 20% final para estimar métricas de erro.

### Por que escolheu utilizar este método?

A validação cruzada é um método conhecido e validado.

### e. Quais evidências você possui de que seu modelo é suficientemente bom?

O modelo LGBM apresentou ganhos em relação a uma regressão linear feita apenas para fins ilustrativos. Além disso, no gráfico de real x preditos, percebe-se que a tendência está sendo seguida adequadamente, e a média está calibrada.
