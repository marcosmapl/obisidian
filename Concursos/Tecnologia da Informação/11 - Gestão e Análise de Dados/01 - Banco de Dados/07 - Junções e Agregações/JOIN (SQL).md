---
disciplina: Tecnologia da Informação
tópico: SQL
created: 2026-01-16T19:10:00
updated: 2026-01-16T19:15:00
---

## Conceito

> [!note] JOIN
> Utilizada para especificar o método de junção (combinação) entre duas tabelas, com base em uma coluna em comum.

#tecnologia_informacao/sql/join

---
## Tipos de JOIN

### INNER JOIN

- Retorna os registro onde houver correspondência de valores em ambas as tabelas (**INTERSECÇÃO**).
### LEFT JOIN

- Retorna todos os registros da tabela da **Esquerda** e seus correspondentes da tabela da **Direita**, para os registros que não houve correspondência será retornado **NULL**.
### RIGHT JOIN

- Retorna todos os registros da tabela da **Direita** e seus correspondentes da tabela da **Esquerda**, para os registros que não houve correspondência será retornado **NULL**.
### FULL OUTER JOIN

- Retorna todos os registros de ambas as tabelas, havendo ou não correspondência de valores.

![[Pasted image 20260116193339.jpg]]

> [!important] A junção de uma tabela com ela mesma é chamada de **SELF JOIN**.

---
## Tópicos Relacionados

- [[FROM (SQL)]]
