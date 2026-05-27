---
disciplina: Tecnologia da Informação
tópico: SQL
created: 2025-12-30T17:03:00
updated: 2026-01-16T19:05:00
---

## Conceito

> [!note] DEFAULT
> A restrição **DEFAULT** é utilizada para **definir um valor padrão** a ser atribuído a uma coluna quando nenhum valor é informado na inserção do registro.

#tecnologia_informacao/sql/ddl/default

---
## Exemplos

### Restrição na criação da tabela

```sql
CREATE TABLE SERVIDOR (  
	ID INT PRIMARY KEY,  
	NOME VARCHAR(50) NOT NULL,  
	SITUACAO VARCHAR(20) DEFAULT 'ATIVO',  
	DATA_CADASTRO DATE DEFAULT CURRENT_DATE  
);
```

### DEFAULT com valor numérico

```sql
CREATE TABLE PRODUTO (  
	ID INT PRIMARY KEY,  
	ESTOQUE INT DEFAULT 0,  
	PRECO DECIMAL(10,2) NOT NULL  
);
```

### Restrição com ALTER TABLE

```sql
ALTER TABLE SERVIDOR  
	ALTER COLUMN SITUACAO SET DEFAULT 'ATIVO';
```

---
## Tópicos Relacionados

- [[CREATE (SQL)]]
- [[ALTER (SQL)]]


