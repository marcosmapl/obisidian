---
disciplina: Tecnologia da Informação
tópico: SQL
created: 2026-01-06T15:49:00
updated: 2026-01-06T15:50:00
---

## Conceito

> [!note] SELECT
> Comando da **DML (Data Manipulation Language)** utilizado para **consultar e recuperar dados** armazenados em uma ou mais tabelas de um banco de dados relacional.

> [!tip] O `SELECT` **não altera os dados**, apenas os **lê**.

#tecnologia_informacao/banco_dados/sql/select

---
## Estrutura Básica

```sql
SELECT coluna1, coluna2
FROM tabela
WHERE condição;
```

---
## Cláusulas Principais

- **SELECT**: Define as colunas ou expressões retornadas;
- **FROM**: Indica a tabela ou conjunto de tabelas;
- **WHERE**: Filtra registros;
- **ORDER BY**: Ordena o resultado;
- **GROUP BY**: Agrupa registros;
- **HAVING**: Filtra grupos agregados.

## Operadores e Recursos Comuns

- **Operadores:**
    - `=`, `<>`, `>`, `<`, `>=`, `<=`
    - `AND`, `OR`, `NOT`

- **Funções de agregação:**
    - `COUNT`, `SUM`, `AVG`, `MIN`, `MAX`

- **Outros recursos:**  
    - `DISTINCT`
    - `JOIN`
    - `LIKE`
    - `IN`
    - `BETWEEN`
    - Subconsultas (`SELECT` aninhado)

---
## Tópicos Relacionados

- [[INSERT (SQL)]]
- [[UPDATE (SQL)]]
- [[DELETE (SQL)]]
- [[WHERE (SQL)]]
- [[JOIN (SQL)]]
- [[GROUP BY (SQL)]]
- [[HAVING (SQL)]]
- [[ORDER BY (SQL)]]
- [[Projeção (Modelo Relacional)]]

