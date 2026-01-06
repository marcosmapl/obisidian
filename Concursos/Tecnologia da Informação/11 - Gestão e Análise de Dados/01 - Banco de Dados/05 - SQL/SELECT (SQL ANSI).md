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

## Pontos de Prova

- `SELECT *` retorna todas as colunas;
- `WHERE` filtra linhas, `HAVING` filtra grupos; 
- `ORDER BY` é processado **após** o `WHERE`;
- Tema recorrente em provas de TI.

---
## Tópicos Relacionados

- [[DML — Data Manipulation Language]]
- [[JOIN]]
- [[GROUP BY]]
- [[WHERE]]
- [[Funções de Agregação SQL]]
