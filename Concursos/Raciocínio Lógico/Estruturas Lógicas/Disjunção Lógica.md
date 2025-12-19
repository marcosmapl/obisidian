---
disciplina: Raciocínio Lógico
tópico: Conceitos Introdutórios
created: 2025-12-15T15:11:00
tags:
  - rlm/conectivos/disjunção
node_size: "10"
---
## 1. Conceito Geral
- A **disjunção** é o conectivo lógico expresso, em regra, pela palavra **“ou”**.
- Divide-se em **dois tipos**:
  - **Disjunção inclusiva**
  - **Disjunção exclusiva**

🧠 **Mnemônico inicial:**  
**OU = pode um, pode outro, depende do tipo**

---

## 2. Disjunção Inclusiva (p ∨ q)

### Conceito
- Conectivo: **“ou” (sentido comum)**
- Símbolo lógico: **∨**
- A proposição composta é **verdadeira se pelo menos uma** das proposições for verdadeira.

📌 **Regra de prova:**  
> Na disjunção inclusiva, **aceita os dois verdadeiros**.

---

### Exemplo
- p: *“Maria foi ao cinema.”*
- q: *“João foi ao parque.”*

📌 Proposição composta:
- **p ∨ q**:  
  *“Maria foi ao cinema **ou** João foi ao parque.”*

➡ Pode ter acontecido:
- Apenas p  
- Apenas q  
- **p e q juntos**

---

### Tabela-Verdade – Disjunção Inclusiva

| p | q | p ∨ q |
|---|---|-------|
| V | V | **V** |
| V | F | **V** |
| F | V | **V** |
| F | F | F |

🧠 **Decoreba:**  
> Só é falsa quando **tudo é falso**.

---

### Palavras Equivalentes (Prova)
- ou  
- ou então  
- e/ou  

➡ **Todas indicam disjunção inclusiva**, salvo contexto contrário.

---

## 3. Disjunção Exclusiva (p ⊻ q)

### Conceito
- Conectivo: **“ou...ou”**
- Símbolo lógico: **⊻**  
  (algumas bancas usam: **≠** ou **(p ∨ q) ∧ ~(p ∧ q)**)

📌 Apenas **uma** proposição pode ser verdadeira.

🧠 **Palavra-chave:** *exclusão*

---

### Exemplo
- p: *“Maria foi ao cinema.”*
- q: *“João foi ao parque.”*

📌 Proposição composta:
- **p ⊻ q**:  
  *“Ou Maria foi ao cinema, ou João foi ao parque.”*

➡ **Não podem ocorrer juntas.**

---

### Tabela-Verdade – Disjunção Exclusiva

| p | q | p ⊻ q |
|---|---|-------|
| V | V | F |
| V | F | **V** |
| F | V | **V** |
| F | F | F |

🧠 **Decoreba:**  
> Exclusivo = **um sim, outro não**

---

## 4. Diferença Essencial (Muito Cobrado)

| Situação | Inclusiva | Exclusiva |
|--------|-----------|-----------|
| Ambos verdadeiros | ✔️ Verdadeiro | ❌ Falso |
| Apenas um verdadeiro | ✔️ Verdadeiro | ✔️ Verdadeiro |
| Ambos falsos | ❌ Falso | ❌ Falso |

---
