---
disciplina: Tecnologia da Informação
tópico: Bloqueios (Locks)
created: 2026-05-22T08:12:59
updated: 2026-05-22T08:12:59
---

- **Deadlock**: o que é e como ocorre.
- Protocolo **2PL (Two-Phase Locking)**.
- Protocolo **2PC (Two-Phase Commit)** para transações distribuídas.
- Tipos de **Locks** (compartilhado/exclusivo) e seu funcionamento.

**Dica de Ouro: Locks = Semáforos do BD!**  
**Locks Compartilhados (Leitura):** Sinal verde para vários carros (transações) passarem lendo, mas sinal vermelho para quem quer alterar a pista (escrever).  
**Locks Exclusivos (Escrita):** Sinal vermelho para todos os outros; só um carro (transação) pode passar e alterar a pista.