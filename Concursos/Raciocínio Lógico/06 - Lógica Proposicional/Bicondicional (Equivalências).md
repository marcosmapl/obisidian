---
disciplina: Raciocínio Lógico
tópico: Equivalências Lógicas
subtópico: Bicondicional
created: 2025-12-24T00:00:00
updated: 2025-12-24T00:00:00
tags:
  - rlm
  - equivalencias
---

## 🔸Definição

> [!note] Bicondicional
> A bicondicional (p ↔ q) representa uma equivalência entre duas proposições, sendo verdadeira quando ambas têm o mesmo valor lógico.

---
## 🔸Fórmulas Principais

#### 1. Definição pela Dupla Condicional
$$p \leftrightarrow q \equiv (p \to q) \land (q \to p)$$

**Leitura**: "p se e somente se q" equivale a "(Se p então q) E (Se q então p)"

#### 2. Equivalência em termos de Disjunção
$$p \leftrightarrow q \equiv (\sim p \lor q) \land (\sim q \lor p)$$

#### 3. Equivalência de Valores Iguais
$$p \leftrightarrow q \equiv (p \land q) \lor (\sim p \land \sim q)$$

**Leitura**: "Ambas verdadeiras OU ambas falsas"

### 🔹Exemplos

#### Exemplo 1 - Dupla Condicional
- **Original**: "Passo no concurso se e somente se estudar"
- **Equivalente**: "(Se passo no concurso, então estudei) E (Se estudei, então passo no concurso)"

#### Exemplo 2 - Valores Iguais
- **Original**: "O número é par se e somente se é divisível por 2"
- **Equivalente**: "(O número é par E é divisível por 2) OU (O número não é par E não é divisível por 2)"

---
## 🔸Tabela - Verdade

| p | q | p↔q | p→q | q→p | (p→q)∧(q→p) | p∧q | ~p∧~q | (p∧q)∨(~p∧~q) |
|---|---|-----|-----|-----|-------------|-----|-------|---------------|
| V | V | V   | V   | V   | V           | V   | F     | V             |
| V | F | F   | F   | V   | F           | F   | F     | F             |
| F | V | F   | V   | F   | F           | F   | F     | F             |
| F | F | V   | V   | V   | V           | F   | V     | V             |

---
## 🔸Negação da Bicondicional

$$\sim(p \leftrightarrow q) \equiv p \leftrightarrow \sim q \equiv \sim p \leftrightarrow q$$

Ou ainda:

$$\sim(p \leftrightarrow q) \equiv (p \land \sim q) \lor (\sim p \land q)$$

**Leitura**: "Não (p se e somente se q)" equivale a "(p E não q) OU (não p E q)" - valores diferentes!

**Exemplo**:
- **Original**: "Viajo se e somente se tenho dinheiro"
- **Negação**: "(Viajo E não tenho dinheiro) OU (Não viajo E tenho dinheiro)"

> [!quote] Negação da Bicondicional
> **Uma verdadeira e outra falsa**

---
## 🔸Propriedades da Bicondicional

#### Comutativa
$$p \leftrightarrow q \equiv q \leftrightarrow p$$

#### Associativa
$$p \leftrightarrow (q \leftrightarrow r) \equiv (p \leftrightarrow q) \leftrightarrow r$$

---
## 🔸Aplicações em Provas
- Identificar condições necessárias e suficientes
- Transformar em dupla condicional
- Entender quando valores devem ser iguais ou diferentes

---
## 🔸Links relacionados

- [[Bicondicional Lógica]]
- [[Condicional (Equivalências)]]
- [[Equivalências Lógicas]]
- [[MOC — Lógica Proposicional]]
