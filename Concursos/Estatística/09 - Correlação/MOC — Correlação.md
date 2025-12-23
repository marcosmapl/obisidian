---
disciplina: Estatística
tópico: Correlação
created: 2025-12-23T00:00:00
progresso: 0
node_size: "10"
tags:
  - estatistica/correlacao
---

## 🔸 Correlação

- [[Correlação]]
- [[Correlação — Conceito]]
- [[Tipos de Correlação]]
- [[Correlação Linear]]
- [[Correlação Positiva e Negativa]]
- [[Coeficiente de Correlação de Pearson]]
- [[Coeficiente de Correlação de Spearman]]
- [[Interpretação da Correlação]]
- [[Diagrama de Dispersão]]
- [[Covariância]]

#estatistica/correlacao

---
## 🔸 Medindo a Associação

> [!info] Definição
> **Correlação** mede o grau e a direção da relação linear entre duas variáveis quantitativas.

**Coeficiente de Correlação de Pearson:**
$$r = \frac{\sum(x_i - \bar{x})(y_i - \bar{y})}{\sqrt{\sum(x_i - \bar{x})^2 \sum(y_i - \bar{y})^2}}$$

ou

$$r = \frac{Cov(X,Y)}{s_X \cdot s_Y}$$

**Propriedades:**
- $-1 \leq r \leq 1$
- $r = 1$: correlação linear positiva perfeita
- $r = -1$: correlação linear negativa perfeita
- $r = 0$: ausência de correlação linear
- $|r| \to 1$: correlação forte
- $|r| \to 0$: correlação fraca

> [!warning] Importante
> Correlação não implica causalidade. Duas variáveis podem estar correlacionadas sem que uma cause a outra.

