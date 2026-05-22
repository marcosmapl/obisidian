---
disciplina: Tecnologia da Informação
tópico: Banco de Dados
created: 2026-05-18T20:35:00
updated: 2026-05-18T20:40:00
---

**Controle de Concorrência:** Mecanismos para gerenciar o acesso simultâneo aos dados por múltiplas transações, evitando problemas como:

- **Atualização Perdida (Lost Update):** Uma transação sobrescreve a alteração de outra transação concorrente.
- **Leitura Suja (Dirty Read):** Uma transação lê dados modificados por outra transação que ainda não foi confirmada (e pode ser desfeita).
- **Leitura Não Repetível (Non-Repeatable Read):** Uma transação lê o mesmo dado duas vezes e obtém valores diferentes porque outra transação o alterou entre as leituras.
- **Leitura Fantasma (Phantom Read):** Uma transação executa uma consulta duas vezes e obtém conjuntos diferentes de linhas porque outra transação inseriu ou removeu linhas que satisfazem a condição da consulta.

Técnicas de Controle de Concorrência:

- **Bloqueios (Locks):** Mecanismo mais comum. Uma transação "bloqueia" um item de dado para impedir que outras transações o acessem de forma conflitante.
    - _Bloqueio Compartilhado (Shared Lock / Read Lock):_ Permite que outras transações leiam, mas não modifiquem o item.
    - _Bloqueio Exclusivo (Exclusive Lock / Write Lock):_ Impede que outras transações leiam ou modifiquem o item.
- **Protocolo de Bloqueio de Duas Fases (2PL - Two-Phase Locking):** Garante serializabilidade. Possui duas fases: crescimento (transação pode adquirir locks, mas não liberar) e encolhimento (transação pode liberar locks, mas não adquirir novos).
- **Deadlock (Impasse):** Situação em que duas ou mais transações esperam indefinidamente umas pelas outras para liberar locks. Requer detecção e resolução (ex: abortar uma transação).
- **Timestamp Ordering:** Atribui um timestamp único a cada transação e ordena as operações com base nesses timestamps.

**Recuperação de Falhas:** Mecanismos para restaurar o BD a um estado consistente após uma falha. Utiliza **Logs de Transação** (registram todas as operações).

**Two-Phase Commit (2PC):** Protocolo para garantir atomicidade em transações distribuídas (que envolvem múltiplos SGBDs/sites).