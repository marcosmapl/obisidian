---
disciplina: Raciocínio Lógico
tópico: Equivalências Lógicas
subtópico: Identidade e Absorção
created: 2025-12-24T00:00:00
updated: 2025-12-24T00:00:00
tags:
  - rlm
  - equivalencias
---

## 🔸Definição

> [!note] Lei de Identidade (Elemento Neutro)
> As Leis de Identidade estabelecem que existem elementos neutros para as operações lógicas (V para conjunção, F para disjunção).

---
## 🔸Fórmulas

#### Identidade da Conjunção (E)
$$p \land V \equiv p$$
$$p \land F \equiv F$$

**Leitura**: 
- "p E Verdadeiro" = p
- "p E Falso" = Falso

#### Identidade da Disjunção (OU)
$$p \lor V \equiv V$$
$$p \lor F \equiv p$$

**Leitura**:
- "p OU Verdadeiro" = Verdadeiro
- "p OU Falso" = p

### 🔹Exemplos

#### Conjunção
- **p ∧ V**: "Está chovendo E é verdade" = "Está chovendo"
- **p ∧ F**: "Está chovendo E é mentira" = Falso (nada pode ser verdadeiro E falso)

#### Disjunção
- **p ∨ V**: "Está chovendo OU é verdade" = Verdadeiro (sempre)
- **p ∨ F**: "Está chovendo OU é mentira" = "Está chovendo"

---
## 🔸Tabela - Verdade

#### Conjunção
| p | V | p∧V | F | p∧F |
|---|---|-----|---|-----|
| V | V | V   | F | F   |
| F | V | F   | F | F   |

#### Disjunção
| p | V | p∨V | F | p∨F |
|---|---|-----|---|-----|
| V | V | V   | F | V   |
| F | V | V   | F | F   |

---
## 🔸Resumo

### Identidade (Elemento Neutro)
| Operação          | Com Verdade (V) | Com Falsidade (F) |
| ----------------- | --------------- | ----------------- |
| **Conjunção (∧)** | p ∧ V ≡ p       | p ∧ F ≡ F         |
| **Disjunção (∨)** | p ∨ V ≡ V       | p ∨ F ≡ p         |
| **2ª Absorção**   | p ∧ (p ∨ q) ≡ p | E absorve OU      |

---
## 🔸Macetes para Lembrar

### Identidade
**"V é neutro do E, F é neutro do OU"**
- Conjunção precisa de V para manter o valor
- Disjunção precisa de F para manter o valor

---
## 🔸Diferenças Importantes

| Lei | Estrutura | Resultado |
|-----|-----------|-----------|
| **Idempotência** | p ∧ p ou p ∨ p | p |
| **Absorção** | p ∧ (p ∨ q) ou p ∨ (p ∧ q) | p |
| **Identidade** | p ∧ V ou p ∨ F | p |

---
## 🔸Links relacionados

- [[Equivalências Lógicas]]
- [[Leis de Idempotência]]
- [[Lei Comutativa]]
- [[MOC — Lógica Proposicional]]
