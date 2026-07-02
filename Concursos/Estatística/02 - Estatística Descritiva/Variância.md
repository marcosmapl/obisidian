---
disciplina: Estatística
tópico: Estatística Descritiva
created: 2026-07-02T05:50:00
updated: 2026-07-02T05:55:00
---

## Conceito

> [!note] Variância
> A variância é determinada pela média dos quadrados dos desvios médios.

---
## Variância Populacional

$$ \sigma^2 = \frac{\sum_{i=1}^n (x_i - \mu)^2}{n} $$

### Simplificação

$$ \sigma^2 = \bar{x^2} - (\bar{x})^2 $$

---
## Variância Amostral


$$ s^2 = \frac{\sum_{i=1}^n (x_i - \bar{x})^2}{n - 1} $$

### Simplificação

$$ s^2 = [ \bar{x^2} - (\bar{x})^2 ] \times (\frac{n}{n - 1}) $$

> [!tip] Amostras Grandes
> Em amostras grandes (n > 30), **não há diferença significativa** entre os resultados proporcionados pela **utilização de qualquer dos dois divisores**, **n ou (n-1)**

---
## Relação entre Variâncias

$$ s^2 = \sigma^2 \times \frac{n}{n-1} $$

---
## Dados Agrupados

### Variância Populacional

$$ \sigma^2 = \frac{\sum_{i=1}^m (x_i - \mu)^2 \times f_i}{n} $$
### Variância Amostral

$$ s^2 = \frac{\sum_{i=1}^n (x_i - \bar{x})^2 \times f_i}{n - 1} $$
