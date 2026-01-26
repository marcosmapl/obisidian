---
disciplina: Tecnologia da Informação
tópico: SQL
created: 2025-12-20T15:24:00
updated: 2026-01-16T18:55:00
---

## Conceito

> [!note] TRUNCATE
> Remove **todos os registros** de uma tabela, mantendo sua estrutura.

#tecnologia_informacao/sql/ddl/truncate

---
## Características importantes

- Mais rápido que **DELETE**
- Não permite cláusula **WHERE**
- Reinicia contadores internos (dependente do SGBD)

---
## Exemplo

```sql
TRUNCATE TABLE aluno;
```

---
## Tópicos Relacionados

- [[DELETE (SQL)]]
- [[DROP (SQL)]]


