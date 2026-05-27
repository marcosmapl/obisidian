---
disciplina: Tecnologia da Informação
tópico: SQL
created: 2025-12-20T15:00:00
---

## Conceito

> [!note] Data Definition Language
> A **DDL (Data Definition Language)** é o subconjunto da linguagem **SQL** responsável por **definir, alterar e remover estruturas do banco de dados**, como tabelas, esquemas, visões e índices.

> [!tip] Os comandos DDL **atuam sobre a estrutura** dos objetos, e não sobre os dados em si.

---
## Principais Comandos da DDL (ANSI SQL)

- [[CREATE (SQL)]]
- [[ALTER (SQL)]]
- [[DROP (SQL)]]
- [[TRUNCATE (SQL)]] _(suportado amplamente, embora não formalmente central no ANSI)_
- [[RENAME (SQL)]] _(varia conforme o SGBD, mas previsto conceitualmente)_
- [[UNIQUE (SQL)]]
- [[PRIMARY KEY (SQL)]]
- [[FOREIGN KEY (SQL)]]
- [[CHECK (SQL)]]
- [[DEFAULT (SQL)]]

---
## Comparação conceitual (DDL × DML)

| Aspecto    | DDL                  | DML                      |
| ---------- | -------------------- | ------------------------ |
| Atua sobre | Estrutura            | Dados                    |
| Objetivo   | Definição de objetos | Manipulação de registros |
| Exemplos   | CREATE, ALTER        | INSERT, UPDATE           |

---
## Observações importantes (prova e prática)

- Comandos DDL **não utilizam WHERE**
- Normalmente implicam **COMMIT implícito**
- Afetam o **catálogo do banco de dados**
- São executados por usuários com **privilégios administrativos**

---
## Tópicos relacionados

- [[DML — Data Manipulation Language]]
- [[DTL — Data Transaction Language]]
- [[DCL — Data Control Language]]
