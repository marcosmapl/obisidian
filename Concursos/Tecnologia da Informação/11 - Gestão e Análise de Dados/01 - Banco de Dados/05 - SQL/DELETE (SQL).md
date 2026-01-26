---
disciplina: Tecnologia da Informação
tópico: SQL
created: 2026-01-16T16:15:00
updated: 2026-01-16T16:20:00
---

## Conceito

> [!note] DELETE
> Comando da **DML (Data Manipulation Language)** utilizado para **remover registros (linhas)** de uma tabela em um banco de dados relacional.

> [!danger] O `DELETE` **remove dados permanentemente**. Sem `WHERE`, **todas as linhas** da tabela serão excluídas.

#tecnologia_informacao/banco_dados/sql/delete

---
## Estrutura Básica

```sql
DELETE FROM tabela
WHERE condição;
```

---
## Cláusulas Principais

- **DELETE FROM**: Define a tabela da qual os dados serão removidos;
- **WHERE**: Filtra quais registros serão excluídos;
- **USING / FROM** (alguns SGBDs): Permite exclusão com base em outras tabelas;
- **SELECT**: Pode ser usado em subconsultas para definir critérios de exclusão.

---
## Operadores e Recursos Comuns

### Exclusão simples

```sql
DELETE FROM clientes WHERE id = 5;
```
### Exclusão condicional

```sql
DELETE FROM pedidos WHERE status = 'cancelado';
```
### Exclusão sem WHERE (⚠️ perigoso)

```sql
DELETE FROM tabela;
```
### Exclusão com subconsulta

```sql
DELETE FROM funcionarios WHERE id IN (     SELECT id     FROM funcionarios     WHERE cargo = 'Estagiário' );
```

---
## Pontos de Prova

- `DELETE` remove **linhas**, não colunas;
- Sem `WHERE`, **todas as linhas** da tabela são excluídas;
- Diferença importante:
    - `DELETE`: remove linhas individualmente (pode usar `WHERE`);
    - `TRUNCATE`: remove **todas** as linhas e é **DDL**;
- Pode violar restrições de **FOREIGN KEY**;
- Muito cobrado em provas de SQL.

---
## Tópicos Relacionados

- [[SELECT (SQL)]]
- [[INSERT (SQL)]]
- [[UPDATE (SQL)]]
- [[TRUNCATE (SQL)]]
- [[WHERE]]
- [[FOREIGN KEY (SQL)]]
- [[TRANSACTION]]