---
disciplina: Tecnologia da Informação
tópico: SQL
created: 2025-12-20T15:18:00
---

> ✏️Modifica a estrutura de um objeto existente.

## 🔸Operações comuns

- Adicionar coluna
- Alterar tipo de dado
- Remover coluna

### 🔹Exemplo — adicionar coluna

```
ALTER TABLE aluno ADD email VARCHAR(150);
```

### 🔹Exemplo — remover coluna

```
ALTER TABLE aluno DROP email;
```

#ti/sql/ddl/alter