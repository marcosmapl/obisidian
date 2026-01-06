---
disciplina: Tecnologia da Informação
tópico: SQL
created: 2025-12-20T15:24:00
---

## Conceito

> [!note] TRUNCATE
> Remove **todos os registros** de uma tabela, mantendo sua estrutura.

#tecnologia_informacao/sql_ansi/ddl/truncate

---
## Características importantes

- Mais rápido que **[[DELETE]]**
- Não permite cláusula **[[WHERE]]**
- Reinicia contadores internos (dependente do SGBD)

---
## Exemplo

```
TRUNCATE TABLE aluno;
```

---
## Navegação

- [[DDL — Data Definition Language]]
- [[SQL ANSI]]
- [[MOC — Gestão e Análise de Dados]]
- [[Tecnologia da Informação]]
