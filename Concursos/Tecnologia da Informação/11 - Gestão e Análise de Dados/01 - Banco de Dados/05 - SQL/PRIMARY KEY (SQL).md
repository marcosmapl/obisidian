---
disciplina: Tecnologia da Informação
tópico: SQL
created: 2025-12-30T15:34:00
updated: 2025-12-30T15:35:00
---

## Conceito

> [!note] PRIMARY KEY
> É uma restrição de integridade utilizada para identificar de forma única cada registro de uma tabela.

Ela impõe, simultaneamente, duas regras fundamentais:

1. **Unicidade** ([[UNIQUE (SQL)]]): não podem existir dois registros com o mesmo valor de chave primária;
2. **Não nulidade** (_NOT NULL_): os valores da chave primária **não podem ser NULL**.

#tecnologia_informacao/sql/ddl/primary_key

---
## Exemplos

### Restrição na criação da tabela

```sql
CREATE TABLE ALUNO (
MATRICULA INT,
CPF VARCHAR(11),
NOME VARCHAR(280),
CONSTRAINT PK_ALUNO PRIMARY KEY (ALUNO_ID)
);
```

```sql
CREATE TABLE ALUNO (
MATRICULA INT PRIMARY KEY,
CPF VARCHAR(11),
NOME VARCHAR(280)
);
```

### Restrição para múltiplas colunas

```sql
CREATE TABLE MATRICULA (
ALUNO_ID INT NOT NULL,
DISCIPLINA_ID INT NOT NULL,
ANO INT NOT NULL,
SEMESTRE INT NOT NULL,
CONSTRAINT PK_MATRICULA PRIMARY KEY (ALUNO_ID, DISCIPLINA_ID, ANO, SEMESTRE)
... 
);
```

### Restrição com ALTER TABLE

```sql
ALTER TABLE PESSOA
ADD PRIMARY KEY (CPF);
```

---
## Tópicos Relacionados

- [[Chave Primária — Conceito]]
- [[FOREIGN KEY (SQL)]]
