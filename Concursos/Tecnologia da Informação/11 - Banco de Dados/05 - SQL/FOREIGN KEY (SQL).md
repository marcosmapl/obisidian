---
disciplina: Tecnologia da Informação
tópico: SQL
created: 2025-12-30T15:42:00
updated: 2025-12-30T15:45:00
---

## Conceito

> [!note] Foreign Key
> A restrição é utilizada para definir uma ou mais colunas como **chaves estrangeiras** e prevenir que alguma ação possa destruir essa ligação entre tabelas.


#tecnologia_informacao/sql/ddl/foreign_key

---
## Características

- FOREIGN KEY garante **integridade referencial**;
- Pode ser declarada **na coluna ou na tabela**;    
- Pode possuir **ações referenciais**;
- Pode ser **simples ou composta**.

---
## Exemplos

### Restrição na criação da tabela

```sql
CREATE TABLE pedido (
	pedido_id INT PRIMARY KEY,
	cliente_id INT,
	data_pedido DATE,
	CONSTRAINT fk_pedido_cliente FOREIGN KEY (cliente_id) REFERENCES cliente (cliente_id)
);
```

```sql
CREATE TABLE pedido (
	pedido_id INT PRIMARY KEY,
	cliente_id INT REFERENCES cliente (cliente_id),
	data_pedido DATE
);
```

### Restrição com ações referenciais (ON DELETE / ON UPDATE)

```sql
CREATE TABLE pedido (
	pedido_id INT PRIMARY KEY,
	cliente_id INT,
	data_pedido DATE,
	CONSTRAINT fk_pedido_cliente FOREIGN KEY (cliente_id) REFERENCES cliente (cliente_id) ON DELETE CASCADE ON UPDATE RESTRICT
);
```
### Restrição para múltiplas colunas

```sql
CREATE TABLE item_pedido (
	pedido_id INT,
	produto_id INT,
	CONSTRAINT fk_item_pedido FOREIGN KEY (pedido_id, produto_id) REFERENCES pedido_produto (pedido_id, produto_id)
);
```

---
## Tópicos Relacionados

- [[PRIMARY KEY (SQL)]]
- [[Chave Estrangeira — Conceito]]
- [[Integridade Referencial]]
