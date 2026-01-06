---
disciplina: Tecnologia da Informação
tópico: Banco de Dados
created: 2026-01-06T16:35:00
updated: 2026-01-06T16:40:00
---

## Conceito

> [!note] Redundância Controlada
> Ocorre quando a **repetição de dados é intencional, planejada e gerenciada**, sendo adotada de forma consciente para **melhorar desempenho, disponibilidade ou simplicidade de consultas**, sem comprometer a integridade das informações.

#tecnologia_informacao/banco_dados/redundancia_controlada

---
## Características

- Redundância **planejada** e **documentada**;
- Existência de regras de controle e sincronização;
- Uso consciente de mecanismos do SGBD;
- Equilíbrio entre **integridade** e **desempenho**.

---
## Objetivos Principais

- Aumentar a **performance de consultas**;
- Reduzir custos de *joins* complexos;
- Facilitar relatórios e análises;
- Atender requisitos de alta disponibilidade.

---
## Mecanismos de Controle

- **Restrições de Integridade** (PK, FK, CHECK);
- **Triggers**;
- **Views materializadas**;
- **Procedures** e regras de negócio;
- Controle transacional (ACID).

---
## Exemplos Comuns

- Armazenar o **total do pedido** além dos itens;
- Campos derivados (ex.: idade calculada periodicamente);
- Tabelas de agregação para BI;
- Dados replicados em sistemas distribuídos.

---
## Relação com Normalização

> [!important]
> A redundância controlada normalmente surge após a normalização, por meio da **desnormalização estratégica**, visando ganhos específicos de desempenho.

---
## Comparação com Redundância Não Controlada

| Aspecto | Redundância Controlada | Redundância Não Controlada |
|------|----------------------|----------------------------|
| Planejamento | Sim | Não |
| Integridade | Preservada | Comprometida |
| Uso | Intencional | Acidental |
| Risco | Baixo | Alto |

---
## Tópicos Relacionados

- [[Redundância Não Controlada]]
- [[Normalização]]
- [[Desnormalização]]
- [[Integridade de Dados]]
- [[Triggers]]
