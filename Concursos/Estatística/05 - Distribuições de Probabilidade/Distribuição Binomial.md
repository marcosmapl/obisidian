

> [!info] Distribuição Binomial
> Quando repetimos um mesmo Ensaio de Bernoulli (isto é, o experimento com 2 resultados possíveis), damos origem à Distribuição Binomial.

- Probabilidade de **sucesso** em cada experimento seja a mesma.
- Os eventos sejam **independentes**.

---
## Função de Distribuição de Probabilidades

$$ P(X = k) = C_n^k \times p^k \times q^{n-k} $$

- [[Combinação]]

### Intervalo de Valores

Podemos calcular também a **probabilidade de um intervalo de valores da variável**, **somando as probabilidades correspondente**s. Por exemplo, a probabilidade de obter 1 OU 2 sucessos, é:

$$ P(X = 1 \cup X = 2) = P(X = 1) + P(X = 2) $$

### Probabilidade Complementar

E, para calcular a probabilidade de =="pelo menos um"== sucesso, é mais fácil calcular a **probabilidade complementar**, isto é, a probabilidade de nenhum:

$$ P(X \ge 1) = 1 - P(X = 0) $$

---
## Esperança

$$ E(X) = n \times p $$

> [!tip] A **esperança binomial** é **n vezes** a **esperança de Bernoulli**

---
## Variância

$$ Var(X) = n \times p \times q = n \times p \times (1 - p) $$


> [!tip] A **variância binomial** é **n vezes** a **variância de Bernoulli**
