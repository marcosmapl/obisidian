---
disciplina: Raciocínio Lógico
tópico: Equivalências Lógicas
created: 2025-12-24T08:24:00
updated: 2025-12-24T00:00:00
  - rlm
  - equivalencias
---

## 🔸Principais Equivalências Lógicas

### 🔹Equivalências Fundamentais

#### 1. Dupla Negação
- [[Dupla Negação]]
  - Negação da negação = proposição original
  - $\sim(\sim p) \equiv p$

#### 2. Leis de De Morgan
- [[Lei de De Morgan]]
  - Negação de conjunção e disjunção
  - $\sim(p \land q) \equiv \sim p \lor \sim q$
  - $\sim(p \lor q) \equiv \sim p \land \sim q$

#### 3. Equivalências da Condicional
- [[Condicional (Equivalências)]]
  - Condicional como disjunção: $p \to q \equiv \sim p \lor q$
  - Contrapositiva: $p \to q \equiv \sim q \to \sim p$
  - Negação: $\sim(p \to q) \equiv p \land \sim q$

#### 4. Equivalências da Bicondicional
- [[Bicondicional (Equivalências)]]
  - Dupla condicional: $p \leftrightarrow q \equiv (p \to q) \land (q \to p)$
  - Valores iguais: $p \leftrightarrow q \equiv (p \land q) \lor (\sim p \land \sim q)$

### 🔹Propriedades Algébricas

#### 5. Lei Comutativa
- [[Lei Comutativa]]
  - **Comutativa**: $p \land q \equiv q \land p$ | $p \lor q \equiv q \lor p$

#### 6. Lei Associativa
- [[Lei Comutativa]]
  - **Associativa**: $p \land (q \land r) \equiv (p \land q) \land r$

#### 7. Lei Distributiva
- [[Lei Comutativa]]: $p \land (q \lor r) \equiv (p \land q) \lor (p \land r)$

#### 8. Leis de Idempotência
- [[Leis de Idempotência]]
  - Repetição não altera: $p \land p \equiv p$ | $p \lor p \equiv p$

#### 9. Lei de Identidade
- [[Lei de Identidade]]
  - **Identidade**: $p \land V \equiv p$ | $p \lor F \equiv p$

#### 10. Lei da Absorção
- [[Lei da Absorção]]
  - **Absorção**: $p \lor (p \land q) \equiv p$ | $p \land (p \lor q) \equiv p$

---
## 🔸Tabela Resumo - Equivalências Essenciais

| Nome | Fórmula | Aplicação |
|------|---------|-----------|
| **Dupla Negação** | $\sim(\sim p) \equiv p$ | Simplificação |
| **De Morgan 1** | $\sim(p \land q) \equiv \sim p \lor \sim q$ | Negar conjunção |
| **De Morgan 2** | $\sim(p \lor q) \equiv \sim p \land \sim q$ | Negar disjunção |
| **Condicional** | $p \to q \equiv \sim p \lor q$ | Transformar condicional |
| **Contrapositiva** | $p \to q \equiv \sim q \to \sim p$ | Inverter condicional |
| **Negação Condicional** | $\sim(p \to q) \equiv p \land \sim q$ | Negar condicional |
| **Bicondicional** | $p \leftrightarrow q \equiv (p \to q) \land (q \to p)$ | Dupla implicação |
| **Comutativa** | $p \land q \equiv q \land p$ | Trocar ordem |
| **Distributiva** | $p \land (q \lor r) \equiv (p \land q) \lor (p \land r)$ | Distribuir termo |
| **Idempotência** | $p \land p \equiv p$ | Eliminar repetição |
| **Absorção** | $p \lor (p \land q) \equiv p$ | Simplificar expressão |

---
## 🔸Macetes para Concursos

### 🔹Para Negar:
1. **Condicional**: "Mantém a primeira E nega a segunda"
2. **De Morgan**: "Distribui a negação E troca o conectivo"

### 🔹Para Equivalência:
1. **Condicional**: "Nega a primeira OU mantém a segunda"
2. **Contrapositiva**: "Inverte E nega"

### 🔹Para Simplificar:
1. **Absorção**: "O de fora absorve o de dentro"
2. **Idempotência**: "Repetir não acrescenta"

---
## 🔸Links relacionados

- [[MOC — Lógica Proposicional]]