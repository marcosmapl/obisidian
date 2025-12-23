---
disciplina: Estatística
tópico: Regressão
created: 2025-12-23T00:00:00
progresso: 0
node_size: "10"
tags:
  - estatistica/regressao
---

## 🔸 Regressão

- [[Regressão]]
- [[Regressão — Conceito]]
- [[Regressão Linear Simples]]
- [[Regressão Linear Múltipla]]
- [[Método dos Mínimos Quadrados]]
- [[Coeficiente de Determinação (R²)]]
- [[Análise e Interpretação da Regressão]]
- [[Resíduos]]
- [[Análise de Resíduos]]
- [[Pressupostos da Regressão]]

#estatistica/regressao

---
## 🔸 Regressão Linear

> [!info] Definição
> **Regressão** é uma técnica estatística que modela a relação entre uma variável dependente (Y) e uma ou mais variáveis independentes (X), permitindo fazer previsões.

**Modelo de Regressão Linear Simples:**
$$Y = \beta_0 + \beta_1 X + \epsilon$$

**Equação Ajustada:**
$$\hat{Y} = b_0 + b_1 X$$

**Coeficientes pelo Método dos Mínimos Quadrados:**
$$b_1 = \frac{\sum(x_i - \bar{x})(y_i - \bar{y})}{\sum(x_i - \bar{x})^2} = r \cdot \frac{s_y}{s_x}$$

$$b_0 = \bar{y} - b_1 \bar{x}$$

**Coeficiente de Determinação:**
$$R^2 = \frac{SQR}{SQT} = r^2$$

Onde:
- $R^2 \in [0,1]$
- Mede o percentual da variação de Y explicado por X
- $R^2 = 0.85$ → 85% da variação é explicada pelo modelo

**Interpretação:**
- $b_1 > 0$: relação positiva (X aumenta → Y aumenta)
- $b_1 < 0$: relação negativa (X aumenta → Y diminui)
- $b_0$: valor esperado de Y quando X = 0

