---
disciplina: Tecnologia da Informação
tópico: SQL
created: 2026-01-06T16:03:00
updated: 2026-01-06T16:10:00
---

## Conceito

> [!note] INSERT
> Comando da **DML (Data Manipulation Language)** utilizado para **inserir novos registros (linhas)** em uma tabela de um banco de dados relacional.

> [!tip] O `INSERT` **acrescenta dados**, sem alterar a estrutura da tabela.

#tecnologia_informacao/banco_dados/sql/insert

---
## Estrutura Básica

### Inserção direta

```sql
INSERT INTO tabela (coluna1, coluna2)
VALUES (valor1, valor2);
```

### Inserção sem especificar colunas

```sql
INSERT INTO tabela 
VALUES (valor1, valor2, valor3);
```

📌 Exige correspondência **exata** entre ordem e quantidade de colunas.

### Inserção a partir de consulta

```sql
INSERT INTO tabela_destino (coluna1, coluna2) SELECT coluna1, coluna2 FROM tabela_origem WHERE condição;
```

---
## Características Importantes

- Insere: 
    - **uma ou várias linhas**;
- Respeita:
    - tipos de dados;
    - restrições (`NOT NULL`, `UNIQUE`, `CHECK`);
    - integridade referencial (FK);
- Sujeito a:
    - **controle transacional** (`COMMIT` / `ROLLBACK`).

---
## Limitações e Cuidados

- Falha se:
    - violar restrições de integridade;
    - omitir coluna `NOT NULL` sem valor padrão;
- Valores não informados:
    - assumem `DEFAULT`, se definido;
    - caso contrário, `NULL`.

---
## Pontos de Prova

- `INSERT` **não substitui** registros existentes;
- Pode inserir dados vindos de `SELECT`;
- Operação DML passível de **rollback** antes do `COMMIT`;
- Tema recorrente em provas de TI.

---
## Tópicos Relacionados

- [[DML — Data Manipulation Language]]
- [[SELECT (SQL)]]
- [[DEFAULT (SQL)]]
- [[Integridade Referencial]]
