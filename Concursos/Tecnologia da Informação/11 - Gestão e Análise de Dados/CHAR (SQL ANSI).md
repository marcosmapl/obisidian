---
disciplina: Tecnologia da Informação
tópico: SQL
created: 2025-12-20T09:23:00
---

## Conceito

> [!note] Char (SQL ANSI)
> O **CHAR** é um tipo de dado do padrão **SQL ANSI** utilizado para armazenar **cadeias de caracteres de comprimento fixo**.

#tecnologia_informacao/sql_ansi/char

---
## Características

- Possui tamanho **fixo** definido na criação (CHAR(n));
- Preenche automaticamente com **espaços à direita** quando o valor armazenado é menor que o tamanho definido;
- Indicado para dados com comprimento padronizado (ex.: códigos).

---
## Exemplos

- `CHAR(2)` para siglas de estados (ex.: `SP`, `RJ`);
- `CHAR(11)` para CPF sem formatação;
- `CHAR(8)` para códigos internos fixos.

---
## Tópicos Relacionados

- [[VARCHAR (SQL ANSI)]]
- [[CLOB (SQL ANSI)]]

---
## Navegação

- [[Tecnologia da Informação]]
- [[MOC — Gestão e Análise de Dados]]
- [[SQL ANSI]]
- [[Tipos Textuais SQL]]
