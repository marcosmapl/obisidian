
- Suponha um exemplo em que sejam dados n pares de valores observados de X e Y. Sejam a e b as estimativas de α e β, respectivamente, teremos a seguinte reta de regressão estimada:

$$ \hat{Y} = \alpha + \beta \cdot X_i $$

- Os desvios (ou erros) entre os valores observados e os valores estimados de Y na reta de regressão são dados por:

$$ \epsilon = Y_i - \hat{Y} $$


- O método dos mínimos quadrados é tal que a **soma dos quadrados dos desvios seja mínima**.

$$ \sum_{i=1}^n{\epsilon_i^2} = \sum^n_{i=1}{(Y_i - \hat{Y}_i)^2} $$

- Por esse método, temos:

$$ \frac{S_{XY}}{S_{XX}} = \frac{COV(X,Y)}{VAR(X)} $$

$$ \alpha = \hat{Y} - \beta \cdot \bar{X} = \frac{\sum^n_{i=1}{Y}}{n} - \beta \cdot \frac{\sum^n_{i=1}{X}}{n} $$