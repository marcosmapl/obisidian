---
disciplina: Raciocínio Lógico
tópico: Equivalências Lógicas
subtópico: Condicional
created: 2025-12-24T00:00:00
updated: 2025-12-24T00:00:00
tags:
  - rlm
  - equivalencias
---

## 🔸Definição

> [!note] Condicional
> A condicional (p → q) pode ser expressa de diferentes formas equivalentes, todas com o mesmo valor lógico.

---
## 🔸Fórmulas Principais

#### 1. Equivalência Fundamental da Condicional
$$p \to q \equiv \sim p \lor q$$

**Leitura**: "Se p então q" equivale a "Não p OU q"

#### 2. Contraposição (Contrapositiva)
$$p \to q \equiv \sim q \to \sim p$$

**Leitura**: "Se p então q" equivale a "Se não q então não p"

### 🔹Exemplos

#### Exemplo 1 - Equivalência Fundamental
- **Original**: "Se chove, então a rua fica molhada"
- **Equivalente**: "Não chove OU a rua fica molhada"

#### Exemplo 2 - Contraposição
- **Original**: "Se estudo, então passo no concurso"
- **Contrapositiva**: "Se não passo no concurso, então não estudei"

---
## 🔸Tabela-Verdade

| p | q | p→q | ~p | ~p∨q | ~q | ~p | ~q→~p |
|---|---|-----|----|----|----|----|-------|
| V | V | V   | F  | V  | F  | F  | V     |
| V | F | F   | F  | F  | V  | F  | F     |
| F | V | V   | V  | V  | F  | V  | V     |
| F | F | V   | V  | V  | V  | V  | V     |

---
## 🔸Negação da Condicional
**Importante**: A negação da condicional NÃO é outra condicional!

$$\sim(p \to q) \equiv p \land \sim q$$

**Leitura**: "Não é verdade que se p então q" equivale a "p E não q"

> [!tip] **Memorizar**: Regra do marido infiél *"Mantém a primeira e nega a segunda"*.

**Exemplo**:
- **Original**: "Se chove, então levo guarda-chuva"
- **Negação**: "Chove E não levo guarda-chuva"

---
## 🔹Aplicações Importantes
- Transformar condicional em disjunção facilita resolução de problemas

---
## 🔸Links relacionados

- [[Bicondicional Lógica]]
- [[Bicondicional (Equivalências)]]
- [[Condicional Lógica]]
- [[Condicional (Equivalências)]]
- [[Equivalências Lógicas]]
- [[MOC — Lógica Proposicional]]
