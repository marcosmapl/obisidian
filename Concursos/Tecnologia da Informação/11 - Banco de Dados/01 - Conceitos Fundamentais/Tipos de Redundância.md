---
disciplina: Tecnologia da Informação
tópico: Banco de Dados
created: 2025-12-12T04:14:00
updated: 2026-01-06T16:31:00
---

## Conceito

> [!note] Redundância de Dados
> Ocorre quando **a mesma informação é armazenada mais de uma vez** no banco de dados, podendo gerar **inconsistências, desperdício de armazenamento e anomalias**, caso não seja devidamente controlada.

> [!tip] Redundância é o **principal problema que a normalização busca eliminar**.

#tecnologia_informacao/banco_dados/redundancia

---
## Classificação dos Tipos de Redundância

- [[Redundância Não Controlada]]
- [[Redundância Controlada]]
- [[Redundância Funcional]]

---
## Relação com Normalização

| Forma Normal | Redundância Eliminada             |
| ------------ | --------------------------------- |
| 1FN          | Repetições e grupos múltiplos     |
| 2FN          | Dependências parciais             |
| 3FN          | Dependências transitivas          |
| BCNF         | Dependências funcionais indevidas |

---
## Pontos de Prova

- Redundância **não controlada** gera inconsistência;
- Redundância **controlada** pode ser aceitável;
- Normalização ≠ eliminação absoluta de redundância;
- Desnormalização é **decisão técnica**, não erro.

---
## Tópicos Relacionados

- [[Normalização — Conceito]]
- [[Anomalias de Dados]]
- [[Dependência de Dados]]
- [[Desnormalização]]
- [[Modelo Relacional]]

