---
disciplina: Tecnologia da Informação
tópico: SQL
created: 2025-12-20T15:00:00
---

A **DDL (Data Definition Language)** é o subconjunto da linguagem **SQL** responsável por **definir, alterar e remover estruturas do banco de dados**, como tabelas, esquemas, visões e índices.

Os comandos DDL **atuam sobre a estrutura** dos objetos, e não sobre os dados em si.

---
## 🔸Principais Comandos da DDL (ANSI SQL)

- **[[CREATE]]**
- **[[ALTER]]**
- **[[DROP]]**
- **[[TRUNCATE]]** _(suportado amplamente, embora não formalmente central no ANSI)_
- **[[RENAME]]** _(varia conforme o SGBD, mas previsto conceitualmente)_

---
## 📊 Comparação conceitual (DDL × DML)

| Aspecto    | DDL                  | DML                      |
| ---------- | -------------------- | ------------------------ |
| Atua sobre | Estrutura            | Dados                    |
| Objetivo   | Definição de objetos | Manipulação de registros |
| Exemplos   | CREATE, ALTER        | INSERT, UPDATE           |

---
## 📌 Observações importantes (prova e prática)

- Comandos DDL **não utilizam WHERE**
- Normalmente implicam **COMMIT implícito**
- Afetam o **catálogo do banco de dados**
- São executados por usuários com **privilégios administrativos**

---
## 🔗 Links relacionados

- [[SQL ANSI]]
- [[DDL]]
- [[DML]]
- [[DTL]]
- [[DCL]]