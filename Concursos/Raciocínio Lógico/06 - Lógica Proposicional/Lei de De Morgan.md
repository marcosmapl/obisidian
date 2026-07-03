---
disciplina: Raciocínio Lógico
tópico: Equivalências Lógicas
created: 2025-12-24T00:00:00
updated: 2025-12-24T00:00:00
  - rlm
  - equivalencias
---

## 🔸Definição

> [!note] Leis de De Morgan
> As Leis de De Morgan estabelecem como negar uma conjunção ou uma disjunção, transformando conectivos "E" em "OU" e vice-versa.

---
## 🔸Fórmulas

#### Primeira Lei (Negação da Conjunção)
$$\sim(p \land q) \equiv \sim p \lor \sim q$$

**Leitura**: "Não (p E q)" equivale a "Não p OU Não q"

#### Segunda Lei (Negação da Disjunção)
$$\sim(p \lor q) \equiv \sim p \land \sim q$$

**Leitura**: "Não (p OU q)" equivale a "Não p E Não q"

### 🔹Exemplos

#### Exemplo 1 - Negação da Conjunção
- **Proposição original**: "João é médico E Maria é engenheira"
- **Negação (De Morgan)**: "João não é médico OU Maria não é engenheira"

#### Exemplo 2 - Negação da Disjunção
- **Proposição original**: "Vou ao cinema OU vou ao teatro"
- **Negação (De Morgan)**: "Não vou ao cinema E não vou ao teatro"

---
## 🔸Tabela-Verdade

| p   | q   | p∧q | ~(p∧q) | ~p  | ~q  | ~p∨~q | p∨q | ~(p∨q) | ~p∧~q |
| --- | --- | --- | ------ | --- | --- | ----- | --- | ------ | ----- |
| V   | V   | V   | F      | F   | F   | F     | V   | F      | F     |
| V   | F   | F   | V      | F   | V   | V     | V   | F      | F     |
| F   | V   | F   | V      | V   | F   | V     | V   | F      | F     |
| F   | F   | F   | V      | V   | V   | V     | F   | V      | V     |

---
## 🔸Macete para Aplicar

1. **Distribua a negação** para cada proposição simples
2. **Troque o conectivo**: 
   - ∧ (E) vira ∨ (OU)
   - ∨ (OU) vira ∧ (E)

---
## 🔸Aplicações em Concursos

- Encontrar negações de proposições compostas
- Simplificar expressões lógicas
- Análise de argumentos

---
## 🔸Links relacionados

- [[Equivalências Lógicas]]
- [[MOC — Lógica Proposicional]]
