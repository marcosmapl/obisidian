---
disciplina: Tecnologia da Informação
tópico: SQL
created: 2025-12-30T15:16:00
updated: 2025-12-30T15:20:00
---

## Conceito

> [!note] NOT NULL
> A restrição **NOT NULL** força a uma coluna a **NÃO aceitar valores nulos**.

#tecnologia_informacao/sql_ansi/not_null

---
## Exemplos

### Restrição na criação da tabela

```
CREATE TABLE ALUNO (
NOME VARCHAR(20) NOT NULL,
CPF INT PRIMARY KEY ,
SEXO CHAR(1) NOT NULL,
DATA_NASCIMENTO DATE NOT NULL
);
```

### Restrição via ALTER TABLE

```
ALTER TABLE ALUNO
MODIFY CIDADE VARCHAR(50) NOT NULL;
```

---
## Navegação

- [[DDL]]
- [[SQL ANSI]]
- [[MOC — Gestão e Análise de Dados]]
- [[Tecnologia da Informação]]
