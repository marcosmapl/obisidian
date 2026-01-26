---
disciplina: Tecnologia da Informação
tópico: SQL
created: 2026-01-16T16:10:00
updated: 2026-01-16T16:15:00
---
## Conceito

> [!note] UPDATE
> Comando da **DML (Data Manipulation Language)** utilizado para **atualizar dados existentes** (valores de colunas) em uma ou mais linhas de uma tabela.

> [!warning] O `UPDATE` **altera dados já armazenados**. Sem `WHERE`, **todas as linhas** da tabela serão atualizadas.

#tecnologia_informacao/banco_dados/sql/update

---
## Estrutura Básica

```sql
UPDATE tabela
SET coluna1 = valor1, coluna2 = valor2
WHERE condição;
```

---
## Cláusulas Principais

- **UPDATE**: Define a tabela que terá os dados alterados;
- **SET**: Indica as colunas e os novos valores;
- **WHERE**: Filtra quais registros serão atualizados;
- **FROM** (alguns SGBDs): Permite atualização com base em outras tabelas;
- **SELECT**: Pode ser usado em subconsultas para definir valores.

---
## Operadores e Recursos Comuns

### Atualização simples

```sql
UPDATE clientes SET status = 'ativo' WHERE id = 10;
```
### Atualização múltipla de colunas

```sql
UPDATE produtos SET preco = 100, estoque = 50 WHERE categoria = 'A';
```
### Atualização sem WHERE (⚠️ perigoso)

```sql
UPDATE tabela SET coluna = valor;
```
### Atualização com subconsulta

```sql
UPDATE funcionarios SET salario = salario * 1.1 WHERE id IN (     SELECT id     FROM funcionarios     WHERE cargo = 'Analista' );
```

---

## Pontos de Prova

- `WHERE` define **quais linhas** serão atualizadas;
- Sem `WHERE`, **todas as linhas** da tabela são afetadas;
- `UPDATE` não altera a estrutura da tabela, apenas os dados;
- Pode violar restrições como **PRIMARY KEY**, **FOREIGN KEY** e **CHECK**;
- Tema clássico em provas de SQL e DML.

---
## Tópicos Relacionados

- [[SELECT (SQL)]]
- [[INSERT (SQL)]]
- [[DELETE (SQL)]]
- [[WHERE]]
- [[PRIMARY KEY (SQL)]]
- [[FOREIGN KEY (SQL)]]
- [[CHECK (SQL)]]
- [[TRANSACTION]]