---
disciplina: Tecnologia da Informação
tópico: SQL
created: 2026-01-18T16:45:00
updated: 2026-01-18T16:50:00
---

## Conceito

> [!note] Union
> Efetuar a **combinação de resultados** de duas ou mais **instruções SELECT**. 

> [!important] Estas instruções devem ter a **mesma estrutura** de colunas!

#tecnologia_informacao/sql/union

---
## Exemplos

### União (simples)

```sql
SELECT NOME_ALUNO
FROM ALUNOS
UNION
SELECT NOME_DEPENDENTE
FROM ALUNOS
```

> [!important] Por padrão o comando UNION elimina linhas (registros) duplicados, ou seja, com mesmo valor.
### União com duplicidade 

```sql
SELECT NOME_ALUNO
FROM ALUNOS
UNION ALL
SELECT NOME_DEPENDENTE
FROM ALUNOS
```

