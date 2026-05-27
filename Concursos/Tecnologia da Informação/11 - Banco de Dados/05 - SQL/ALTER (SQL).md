---
disciplina: Tecnologia da Informação
tópico: SQL
created: 2025-12-20T15:18:00
updated: 2026-01-16T15:35:00
---

## Conceito

> [!note] ALTER
> Modifica a estrutura de um objeto existente.

#tecnologia_informacao/sql/ddl/alter

---
## Operações comuns

- Adicionar coluna
- Alterar tipo de dado
- Remover coluna

---
## Exemplos

### Adicionar coluna

```sql
ALTER TABLE aluno ADD email VARCHAR(150);
```

### Remover coluna

```sql
ALTER TABLE aluno DROP email;
```

---
## Tópicos Relacionados

- [[CREATE (SQL)]]
