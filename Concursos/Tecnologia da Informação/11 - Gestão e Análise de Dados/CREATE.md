---
disciplina: Tecnologia da Informação
tópico: SQL
created: 2025-12-20T15:16:00
---

> ✏️Cria novos objetos no banco de dados.

## 🔸Uso comum

- Criar tabelas
- Criar visões
- Criar esquemas

### 🔹Exemplo — criação de tabela

```
CREATE TABLE aluno (     
id INTEGER,     
nome VARCHAR(100),     
data_nascimento DATE 
);
```

### 🔹Exemplo — criação de visão

```
CREATE VIEW vw_alunos AS SELECT id, nome FROM aluno;
```

#ti/sql/ddl/create
#ti/sql/ddl/create/table
#ti/sql/ddl/create/view