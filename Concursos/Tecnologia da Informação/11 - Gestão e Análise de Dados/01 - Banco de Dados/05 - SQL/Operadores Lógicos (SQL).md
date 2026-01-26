---
disciplina: Tecnologia da Informação
tópico: SQL
created: 2026-01-16T19:50:00
updated: 2026-01-16T19:50:00
---

## Operadores

| Operador    | Descrição                                           | Exemplo                                                                  |
| ----------- | --------------------------------------------------- | ------------------------------------------------------------------------ |
| **AND**     | E lógico (**conjunção**)                            | ... WHERE altura > 1.60 **AND** idade < 40;                              |
| **OR**      | OU lógico (**disjunção**)                           | ... WHERE velocidade > 60 **OR** velocidade < 40;                        |
| **NOT**     | Inverte o valor lógico (**negação**)                | ... WHERE **NOT** excluido = True;                                       |
| **BETWEEN** | Intervalo **inclusivo**                             | ... WHERE valor **BETWEEN** 150.00 AND 300.00;                           |
| **LIKE**    | Comparação para texto                               | ... WHERE cidade **LIKE** 'são%';                                        |
| **IN**      | Verifica se o valor está num Intervalo especificado | ... WHERE codigo **IN** (1,2,3,5,7);                                     |
| **IS NULL** | Testa se o valor é nulo                             | ... WHERE cnh **IS NULL**;                                               |
| **EXISTS**  | Testa se uma subconsulta retorna algum registro     | ... WHERE **EXISTS** (SELECT NOME_CIDADE FROM CIDADES WHERE IS_CAPITAL); |

---
## Tópicos Relacionados

- [[Operadores Relacionais (SQL)]]
