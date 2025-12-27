---
disciplina: Raciocínio Lógico
tópico: Equivalências Lógicas
subtópico: Propriedades Algébricas
created: 2025-12-24T00:00:00
updated: 2025-12-24T00:00:00
tags:
  - rlm
  - equivalencias
---

## 🔸Definição

> [!note] Definição
> Um termo pode ser distribuído entre operações, similar à distributiva na multiplicação.

___
## 🔸Fórmulas

### 🔹Distributiva do E sobre o OU
$$p \land (q \lor r) \equiv (p \land q) \lor (p \land r)$$

**Leitura**: "p E (q OU r)" equivale a "(p E q) OU (p E r)"

### 🔹Distributiva do OU sobre o E
$$p \lor (q \land r) \equiv (p \lor q) \land (p \lor r)$$

**Leitura**: "p OU (q E r)" equivale a "(p OU q) E (p OU r)"

### 🔹Exemplos

#### Exemplo 1 - Distributiva do E sobre o OU
- **Original**: "Estudo matemática E (faço questões OU assisto aulas)"
- **Equivalente**: "(Estudo matemática E faço questões) OU (Estudo matemática E assisto aulas)"

#### Exemplo 2 - Distributiva do OU sobre o E
- **Original**: "Vou viajar OU (tenho folga E tenho dinheiro)"
- **Equivalente**: "(Vou viajar OU tenho folga) E (Vou viajar OU tenho dinheiro)"

> [!quote] Macete para Prova
> **"Multiplica por todos"** - similar à matemática.
> ⚠️ Cuidado: na lógica, OU também distribui sobre E!

---
## 🔸Tabela - Verdade

### 🔹Lei Distributiva (E sobre OU)
| p   | q   | r   | q∨r | p∧(q∨r) | p∧q | p∧r | (p∧q)∨(p∧r) |
| --- | --- | --- | --- | ------- | --- | --- | ----------- |
| V   | V   | V   | V   | V       | V   | V   | V           |
| V   | V   | F   | V   | V       | V   | F   | V           |
| V   | F   | V   | V   | V       | F   | V   | V           |
| V   | F   | F   | F   | F       | F   | F   | F           |
| F   | V   | V   | V   | F       | F   | F   | F           |
| F   | V   | F   | V   | F       | F   | F   | F           |
| F   | F   | V   | V   | F       | F   | F   | F           |
| F   | F   | F   | F   | F       | F   | F   | F           |

---
## 🔸Comparação com Álgebra

| Propriedade  | Lógica (∧)            | Lógica (∨)            | Álgebra (×)           | Álgebra (+) |
| ------------ | --------------------- | --------------------- | --------------------- | ----------- |
| Distributiva | p∧(q∨r) = (p∧q)∨(p∧r) | p∨(q∧r) = (p∨q)∧(p∨r) | a×(b+c) = (a×b)+(a×c) | -           |

---
## 🔸Links relacionados

- [[Equivalências Lógicas]]
- [[Lei de De Morgan]]
- [[Lei Associativa]]
- [[Lei Comutativa]]
- [[MOC — Lógica Proposicional]]
