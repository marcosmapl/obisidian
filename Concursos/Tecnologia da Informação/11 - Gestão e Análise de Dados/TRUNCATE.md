---
disciplina: Tecnologia da Informação
tópico: SQL
created: 2025-12-20T15:24:00
---

> ✏️Remove **todos os registros** de uma tabela, mantendo sua estrutura.

### 🔹Características importantes

- Mais rápido que **[[DELETE]]**
- Não permite cláusula **[[WHERE]]**
- Reinicia contadores internos (dependente do SGBD)

### 🔹Exemplo

```
TRUNCATE TABLE aluno;
```

#ti/sql/ddl/truncate