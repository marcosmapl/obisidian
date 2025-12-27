---
disciplina: Raciocínio Lógico
tópico: Equivalências Lógicas
subtópico: Idempotência
created: 2025-12-24T00:00:00
updated: 2025-12-24T00:00:00
tags:
  - rlm
  - equivalencias
---

## 🔸Definição

> [!note] Idempotência 
> Significa que repetir a mesma operação não altera o resultado. Uma proposição combinada consigo mesma (E ou OU) resulta na própria proposição.

---
## 🔸Fórmulas

### 🔹Idempotência da Conjunção (E)
$$p \land p \equiv p$$

**Leitura**: "p E p" equivale a "p"

### 🔹Idempotência da Disjunção (OU)
$$p \lor p \equiv p$$

**Leitura**: "p OU p" equivale a "p"

---
## 🔸Exemplos

### 🔹Exemplo 1 - Conjunção
- **Expressão**: "Estudo matemática E estudo matemática"
- **Simplificação**: "Estudo matemática"
- **Análise**: Dizer a mesma coisa duas vezes não muda o fato

### 🔹Exemplo 2 - Disjunção
- **Expressão**: "Vou ao cinema OU vou ao cinema"
- **Simplificação**: "Vou ao cinema"
- **Análise**: Repetir a opção não cria uma nova possibilidade

### 🔹Exemplo 3 - Expressão Composta
- **Expressão**: $(p \land q) \lor (p \land q)$
- **Simplificação**: $p \land q$
- **Aplicação**: Idempotência da disjunção

---
## 🔸Tabela - Verdade

| p | p∧p | p∨p |
|---|-----|-----|
| V | V   | V   |
| F | F   | F   |

**Observação**: As colunas p, p∧p e p∨p são idênticas, confirmando as equivalências.

---
## 🔸Aplicações Práticas

### 🔹Simplificação de Circuitos Lógicos

```
p ∧ p = p  →  Elimina portas lógicas redundantes
p ∨ p = p  →  Reduz complexidade do circuito
```

### 🔹Otimização de Expressões

**Antes**: $(p \land q) \lor (p \land q) \lor r$
**Depois**: $(p \land q) \lor r$

### 🔹Análise de Redundância

Identifica quando informações repetidas não agregam valor lógico

---
## 🔸Comparação com Outras Leis

| Lei | Fórmula | Conceito |
|-----|---------|----------|
| **Idempotência** | p∧p ≡ p | Repetição não altera |
| **Identidade** | p∧V ≡ p | Elemento neutro |
| **Absorção** | p∨(p∧q) ≡ p | Uma expressão absorve outra |

---
## 🔸Macete para Lembrar

**"Repetir não acrescenta nada"**
- Dizer "sim E sim" = "sim"
- Dizer "sim OU sim" = "sim"

**Analogia**:
- Conjunção: "Tenho R$100 E tenho R$100" = "Tenho R$100"
- Disjunção: "Quero café OU quero café" = "Quero café"

---
## 🔸Diferença Importante

### ⚠️ Não confundir com:

- **Tautologia** (sempre verdadeira): $p \lor \sim p \equiv V$
- **Contradição** (sempre falsa): $p \land \sim p \equiv F$

A idempotência usa a **mesma proposição** sem negação.

---
## 🔸Aplicações

- Simplificação de expressões lógicas
- Redução de complexidade em demonstrações

---
## 🔸Exercício Rápido

**Simplifique:**
1. $(p \lor q) \land (p \lor q)$ = ?
2. $[(p \land q) \lor r] \lor [(p \land q) \lor r]$ = ?

**Respostas:**
1. $p \lor q$ (idempotência da conjunção)
2. $(p \land q) \lor r$ (idempotência da disjunção)

---
## 🔸Links relacionados

- [[Equivalências Lógicas]]
- [[Lei Comutativa]]
- [[Lei de Identidade]]
- [[MOC — Lógica Proposicional]]
