---
disciplina: Tecnologia da Informação
tópico: Banco de Dados
created: 2025-12-30T17:00:00
updated: 2025-12-30T17:05:00
---
## Conceito

> [!note] CHECK
> A restrição **CHECK** é utilizada para **definir condições lógicas** que os valores de uma coluna ou conjunto de colunas devem satisfazer, garantindo a **validade dos dados** conforme regras de domínio ou de negócio.

#tecnologia_informacao/sql_ansi/ddl/check

---
## Exemplos

### Restrição na criação da tabela

```
CREATE TABLE SERVIDOR (  
	ID INT PRIMARY KEY,  
	IDADE INT CHECK (IDADE >= 18),  
	SALARIO DECIMAL(10,2) CHECK (SALARIO > 0)  
);
```

### Restrição envolvendo múltiplas colunas

```
CREATE TABLE CONTRATO (  
	DATA_INICIO DATE NOT NULL,  
	DATA_FIM DATE,  
	CHECK (DATA_FIM IS NULL OR DATA_FIM > DATA_INICIO)  
	);
```

### Restrição com ALTER TABLE

```
ALTER TABLE SERVIDOR  
	ADD CONSTRAINT CK_IDADE CHECK (IDADE >= 18);
```

---
## Navegação

- [[DDL]]
- [[SQL ANSI]]
- [[MOC — Gestão e Análise de Dados]]
- [[Tecnologia da Informação]]