---
disciplina: Tecnologia da Informação
tópico: SQL
created: 2025-12-30T15:05:00
updated: 2025-12-30T15:10:00
---

## Conceito

> [!note] DML (Data Manipulation Language)
> Conjunto de comandos do **SQL padrão ANSI** utilizados para **manipular os dados armazenados nas tabelas**, permitindo **consultar, inserir, alterar e excluir registros**, sem modificar a estrutura do banco de dados.

> [!tip] DML atua sobre os **dados**, não sobre o **schema**.

#tecnologia_informacao/banco_dados/sql/dml

![[Pasted image 20260106154249.png]]

---
## Principais Comandos da DML (ANSI SQL)

- SELECT
- INSERT
- UPDATE
- DELETE

---
## Cláusulas

- FROM
- WHERE

---
## Características Importantes

- Afetam:
  - **linhas (tuplas)** das tabelas;
- Sujeitos a:
  - **controle transacional** (`COMMIT`, `ROLLBACK`);
  - restrições de integridade (PK, FK, CHECK);
- Dependem de:
  - permissões de acesso (GRANT).

---
## Pontos de Prova

- `SELECT` é DML no padrão ANSI;
- DML **não altera estrutura**, apenas dados;
- Operações DML podem ser **desfeitas** antes do `COMMIT`;
- Tema recorrente em provas de TI e concursos.

---
## Tópicos Relacionados

- [[SELECT (SQL)]]
- [[INSERT (SQL)]]
- [[UPDATE (SQL)]]
- [[DELETE (SQL)]]
- [[FROM (SQL)]]
- [[WHERE (SQL)]]
- [[DDL — Data Definition Language]]
- [[DCL — Data Control Language]]
- [[TCL — Transaction Control Language]]

