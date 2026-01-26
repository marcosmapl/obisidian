---
disciplina: Tecnologia da Informação
tópico: SQL
created: 2026-01-18T15:30:00
updated: 2026-01-18T15:30:00
---
## Conceito

> [!note] Cláusula Having
> **Filtra agrupamentos** com base numa **condição**.

> [!tip] Só pode existir se houver anteriormente uma cláusula **GROUP BY**.

---
## Exemplos

### Contagem

```sql
SELECT CIDADE, COUNT(CPF) 
FROM ALUNOS
GROUP BY CIDADE 
HAVING COUNT(CPF) > 1;
```

---
## Tópicos Relacionados

- [[GROUP BY (SQL)]]
- [[WHERE (SQL)]]
