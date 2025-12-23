---
disciplina: Estatística
tópico: Inferência Estatística
created: 2025-12-23T00:00:00
progresso: 0
node_size: "10"
tags:
  - estatistica/inferencia
---

## 🔸 Inferência Estatística

- [[Inferência Estatística]]
- [[Inferência Estatística — Conceito]]
- [[Estimação de Parâmetros]]
- [[Estimadores]]
- [[Propriedades dos Estimadores]]
- [[Intervalos de Confiança]]
- [[Intervalo de Confiança para Média]]
- [[Intervalo de Confiança para Proporção]]
- [[Intervalo de Confiança para Variância]]

#estatistica/inferencia

---
## 🔸 Testes de Hipóteses

- [[Testes de Hipóteses]]
- [[Hipótese Nula e Alternativa]]
- [[Testes para Médias]]
- [[Testes para Proporções]]
- [[Testes para Variância]]
- [[Teste Z]]
- [[Teste t]]
- [[Teste Qui-Quadrado]]
- [[Erros Tipo I e Tipo II]]
- [[Nível de Significância]]
- [[Valor-p]]
- [[Região Crítica]]

#estatistica/testes-hipoteses

---
## 🔸 Fundamentos da Inferência

> [!info] Objetivo
> **Inferência Estatística** permite fazer conclusões sobre uma população com base em dados amostrais.

**Intervalo de Confiança para Média ($\sigma$ conhecido):**
$$IC(\mu, 1-\alpha) = \bar{x} \pm z_{\alpha/2} \cdot \frac{\sigma}{\sqrt{n}}$$

**Intervalo de Confiança para Média ($\sigma$ desconhecido):**
$$IC(\mu, 1-\alpha) = \bar{x} \pm t_{\alpha/2} \cdot \frac{s}{\sqrt{n}}$$

**Teste de Hipóteses:**
1. Formular $H_0$ e $H_1$
2. Escolher nível de significância $\alpha$
3. Calcular estatística de teste
4. Tomar decisão (rejeitar ou não rejeitar $H_0$)

**Erros:**
- **Tipo I**: Rejeitar $H_0$ quando é verdadeira (α)
- **Tipo II**: Não rejeitar $H_0$ quando é falsa (β)

