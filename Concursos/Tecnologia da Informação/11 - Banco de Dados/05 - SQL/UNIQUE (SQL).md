---
disciplina: Tecnologia da Informação
tópico: SQL
created: 2025-12-30T15:23:00
updated: 2026-01-16T15:25:00
---

## Conceito

> [!note] UNIQUE
> A restrição **UNIQUE** garante que todos os valores da coluna sejam diferentes, ou seja, **NÃO existam valores repetidos**.

#tecnologia_informacao/sql/ddl/unique

---
## Exemplos

### Restrição na criação da tabela

```sql
CREATE TABLE PESSOA (
NOME VARCHAR(20) NOT NULL,
CPF INT PRIMARY KEY,
CNH VARCHAR(30) UNIQUE,
);
```

### Restrição para múltiplas colunas

```sql
CREATE TABLE MATRICULA (
ALUNO_ID INT NOT NULL,
DISCIPLINA_ID INT NOT NULL,
ANO INT NOT NULL,
SEMESTRE INT NOT NULL,
CONSTRAINT UNIQUE_MATRICULA UNIQUE (ALUNO_ID, DISCIPLINA_ID, ANO, SEMESTRE)
... 
);
```

### Restrição com ALTER TABLE

```sql
ALTER TABLE PESSOA
ADD UNIQUE (CPF);
```

---
## Tópicos Relacionados

- [[Chave Primária — Conceito]]
- [[CHECK (SQL)]]
