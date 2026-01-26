---
disciplina: Tecnologia da Informação
tópico: SQL
created: 2026-01-18T15:20:00
updated: 2026-01-18T15:25:00
---
## Conceito

> [!note] Cláusula Group By
> Foi criada para permitir agregações após a consulta. Pode ser combinada com quantidades, somas, valores máximos, valores mínimos, médias, etc.

---
## Exemplos

### Contagem

```sql
SELECT CIDADE, COUNT(CPF)
FROM ALUNOS
GROUP BY CIDADE;
```

### Somatório

```sql
SELECT CIDADE, SUM(VALOR_PAGO) 
FROM ALUNOS
GROUP BY CIDADE;
```

### Máximo e Mínimo

```sql
SELECT CIDADE, MAX(VALOR_PAGO), MIN(VALOR_PAGO)
FROM ALUNOS
GROUP BY CIDADE;
```

### Média

```sql
SELECT CIDADE, AVG(VALOR_PAGO)
FROM ALUNOS
GROUP BY CIDADE;
```


---
## Tópicos Relacionados

- [[HAVING (SQL)]]
- [[WHERE (SQL)]]
