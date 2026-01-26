---
disciplina: Tecnologia da Informação
tópico: SQL
created: 2025-12-20T15:16:00
---

## Conceito

> [!note] CREATE
> Cria novos objetos no banco de dados.

#tecnologia_informacao/sql/ddl/create

---
## Uso comum

- Criar tabelas
- Criar visões
- Criar esquemas

---
## Exemplos

### Criação de tabela

```sql
CREATE TABLE aluno (     
id INTEGER,     
nome VARCHAR(100),     
data_nascimento DATE 
);
```

#tecnologia_informacao/sql/ddl/create/table
### Criação de visão

```sql
CREATE VIEW vw_alunos AS SELECT id, nome FROM aluno;
```

#tecnologia_informacao/sql/ddl/create/view

---
## Tópicos Relacionados

- [[PRIMARY KEY (SQL)]]
- [[FOREIGN KEY (SQL)]]
- [[ALTER (SQL)]]
