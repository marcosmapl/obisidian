---
disciplina: Tecnologia da Informação
tópico: Banco de Dados
created: 2026-01-12T22:20:00
updated: 2026-01-12T22:30:00
---

## Conceito

> [!note] Normalização
> **Normalização** é o processo de **organizar os dados em tabelas** de forma estruturada, com o objetivo de **eliminar redundâncias**, **evitar anomalias** (inserção, atualização e exclusão) e **garantir integridade e consistência** dos dados.

> [!important] A normalização não eliminar a redundância, pois em determinados cenários, quando controlada, ela é aceitável e até desejada.

#tecnologia_informacao/banco_dados/normalizacao

---
## Objetivos Principais

- **Reduzir redundância de dados**
- **Evitar inconsistências**
- **Facilitar manutenção e evolução do banco**
- **Preservar integridade lógica**
- **Garantir dependências corretas entre atributos**

---
### Anomalias Evitadas

- **Inserção**: impossibilidade de inserir dados sem informações desnecessárias.
- **Atualização**: necessidade de alterar o mesmo dado em vários registros.
- **Exclusão**: perda de informações relevantes ao excluir um registro.

---
## Formas Normais

### 1FN

- É atingida quando todos os **ATRIBUTOS SÃO ATÔMICOS**, ou seja, não existem atributos ==MULTIVALORADOS== ou ==COMPOSTOS==.

### 2FN

- **1FN** + sem **dependência parcial**
- Todos os **atributos NÃO CHAVE** devem depender **completamente da Chave Primária** (composta)

> [!tip] Aplica-se especialmente a tabelas com **chave primária composta**.

### 3FN

- **2FN** + sem **dependência transitória**
- - Todos os **atributos NÃO CHAVE** não podem depender de outros atributos **NÃO CHAVE**.
- Não são permitidos ==CAMPOS CALCULADOS==.

### Forma Normal de Boyce Codd (FNBC)

- Versão mais **rigorosa da 3FN**
- **3FN** + Todo **DETERMINANTE** deve ser **Chave Candidata** (**Superchave**)
### 4FN

- **3FN** + sem **dependência multivalorada**

### 5FN

- **4FN** + sem **dependência de junção**

---
## Normalização × Desnormalização

|Normalização|Desnormalização|
|---|---|
|Menos redundância|Mais redundância|
|Mais integridade|Mais performance em leitura|
|Mais joins|Menos joins|
|OLTP|OLAP / Data Warehouse|

---
## Tópicos Relacionados

- [[Dependência Parcial]]
- [[Dependência Transitiva]]
- [[Chave Composta — Conceito]]
- [[Chave Candidata — Conceito]]
- [[Chave Primária — Conceito]]
- [[Anomalias de Dados]]
