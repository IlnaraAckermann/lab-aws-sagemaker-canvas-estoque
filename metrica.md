Avaliar um modelo de regressão envolve o uso de várias métricas importantes que fornecem insights sobre o desempenho do modelo em relação aos dados reais. Aqui estão algumas das métricas mais comuns:

### R² (R-quadrado)
O coeficiente de determinação, R², indica a proporção da variância nos dados que é explicada pelo modelo. Ele varia de 0 a 1, onde 1 indica um ajuste perfeito do modelo aos dados.

$$ R^2 = 1 - \frac{SS_{res}}{SS_{tot}} $$
- $SS_{res}$ é a soma dos quadrados dos resíduos.
- $SS_{tot}$ é a soma total dos quadrados.

Quanto mais próximo de 1 o valor de R², melhor o modelo se ajusta aos dados.

### Erro Absoluto Médio (MAE)

O Erro Absoluto Médio é a média das diferenças absolutas entre os valores reais e os valores preditos.
O Erro Absoluto Médio (MAE) é dado por:

$$ MAE = \frac{1}{n} \sum_{i=1}^{n} |y_i - \hat{y}_i| $$

- $y_i$ são os valores reais.
- $\hat{y}_i$ são os valores preditos.

Quanto menor o MAE, melhor é o desempenho preditivo do modelo.

### Erro Percentual Médio Absoluto (MAPE)

O Erro Percentual Médio Absoluto expressa o erro médio como uma porcentagem do valor real.

$$ MAPE = \frac{100}{n} \sum_{i=1}^{n} \left|\frac{y_i - \hat{y}_i}{y_i}\right| $$

- $y_i$ são os valores reais.
- $\hat{y}_i$ são os valores preditos.
- Evita a divisão por zero adicionando um pequeno valor ($\epsilon$) ao denominador.
- É útil para entender o erro relativo em diferentes escalas de dados.


### Erro Quadrático Médio (MSE)

O Erro Quadrático Médio é a média das diferenças quadráticas entre os valores reais e os valores preditos.

$$ MSE = \frac{1}{n} \sum_{i=1}^{n} (y_i - \hat{y}_i)^2 $$

- $y_i$ são os valores reais.
- $\hat{y}_i$ são os valores preditos.


### Raiz do Erro Quadrático Médio (RMSE)
A Raiz do Erro Quadrático Médio é a raiz quadrada do MSE, o que a torna na mesma unidade que os valores originais.

$$ RMSE = \sqrt{MSE} $$

- $MSE$ é o Erro Quadrático Médio.
