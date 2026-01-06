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

- [[SELECT (SQL ANSI)]]
- [[INSERT]]

---
### 🔹 INSERT
- **Insere novos registros** em uma tabela;
- Pode inserir:
  - valores diretos;
  - resultados de consultas (`INSERT INTO ... SELECT`).

---
### 🔹 UPDATE
- **Altera dados existentes** em uma tabela;
- Normalmente combinado com `WHERE` para evitar alterações globais.

---
### 🔹 DELETE
- **Remove registros** de uma tabela;
- Pode ser:
  - seletivo (`WHERE`);
  - total (sem `WHERE`).

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
## DML × Outros Subconjuntos do SQL

- **DDL** → definição de estrutura (CREATE, ALTER, DROP);
- **DCL** → controle de acesso (GRANT, REVOKE);
- **TCL** → controle de transações (COMMIT, ROLLBACK, SAVEPOINT).

---
## Pontos de Prova

- `SELECT` é DML no padrão ANSI;
- DML **não altera estrutura**, apenas dados;
- Operações DML podem ser **desfeitas** antes do `COMMIT`;
- Tema recorrente em provas de TI e concursos.

---
## Tópicos Relacionados

- [[DDL — Data Definition Language]]
- [[DCL — Data Control Language]]
- [[TCL — Transaction Control Language]]
- [[SQL ANSI]]
- [[Banco de Dados Relacional]]
