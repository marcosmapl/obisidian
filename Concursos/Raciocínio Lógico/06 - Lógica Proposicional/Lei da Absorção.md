---
disciplina: Raciocínio Lógico
tópico: Equivalências Lógicas
created: 2025-12-24T00:00:00
updated: 2025-12-24T00:00:00
  - rlm
  - equivalencias
---

## 🔸Definição

> [!note] Lei de Absorção
> Uma proposição "absorve" uma expressão mais complexa que a contém, simplificando a expressão lógica.

---
## 🔸Fórmulas

#### Primeira Lei de Absorção
$$p \lor (p \land q) \equiv p$$

**Leitura**: "p OU (p E q)" = p

**Explicação**: Se p é verdadeiro, a expressão toda é verdadeira independente de q. Se p é falso, ambos os lados são falsos.

#### Segunda Lei de Absorção
$$p \land (p \lor q) \equiv p$$

**Leitura**: "p E (p OU q)" = p

**Explicação**: Para a conjunção ser verdadeira, p precisa ser verdadeiro. O resto não importa.

### 🔹Exemplos

#### Exemplo 1 - Primeira Lei
- **Expressão**: "Vou à praia OU (Vou à praia E está sol)"
- **Simplificação**: "Vou à praia"
- **Análise**: Se já vou à praia, não importa se tem sol

#### Exemplo 2 - Segunda Lei
- **Expressão**: "Estudo matemática E (Estudo matemática OU estudo português)"
- **Simplificação**: "Estudo matemática"
- **Análise**: Para o "E" ser verdadeiro, preciso estudar matemática de qualquer forma

#### Exemplo 3 - Aplicação Prática
- **Expressão**: $(p \land q) \lor p$
- **Comutativa**: $p \lor (p \land q)$
- **Absorção**: $p$

---
## 🔸Tabelas-Verdade

#### Primeira Lei: p ∨ (p ∧ q) ≡ p
| p | q | p∧q | p∨(p∧q) |
|---|---|-----|---------|
| V | V | V   | V       |
| V | F | F   | V       |
| F | V | F   | F       |
| F | F | F   | F       |

#### Segunda Lei: p ∧ (p ∨ q) ≡ p
| p | q | p∨q | p∧(p∨q) |
|---|---|-----|---------|
| V | V | V   | V       |
| V | F | V   | V       |
| F | V | V   | F       |
| F | F | F   | F       |

---
## 🔸Resumo

### 🔹Absorção
| Lei | Fórmula | Conceito |
|-----|---------|----------|
| **1ª Absorção** | p ∨ (p ∧ q) ≡ p | OU absorve E |
| **2ª Absorção** | p ∧ (p ∨ q) ≡ p | E absorve OU |

---
## 🔸Macetes para Lembrar

### Absorção
**"O de fora absorve o de dentro"**
- Se p está sozinho fora E dentro de parênteses
- O p sozinho "vence"

---
## 🔸Diferenças Importantes

| Lei              | Estrutura                  | Resultado |
| ---------------- | -------------------------- | --------- |
| **Idempotência** | p ∧ p ou p ∨ p             | p         |
| **Absorção**     | p ∧ (p ∨ q) ou p ∨ (p ∧ q) | p         |
| **Identidade**   | p ∧ V ou p ∨ F             | p         |

---
## 🔸Links relacionados

- [[Equivalências Lógicas]]
- [[Leis de Idempotência]]
- [[Lei Comutativa]]
- [[MOC — Lógica Proposicional]]
