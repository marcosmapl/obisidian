---
disciplina: Tecnologia da Informação
tópico: Banco de Dados
created: 2026-01-06T16:40:00
updated: 2026-01-06T16:45:00
---

## Conceito

> [!note] Redundância Funcional
> Ocorre quando um **atributo pode ser obtido a partir de outro(s)** por meio de uma **dependência funcional**, tornando seu armazenamento **desnecessário do ponto de vista lógico**, embora possa existir fisicamente.

#tecnologia_informacao/banco_dados/redundancia_funcional

---
## Fundamentação Teórica

- Baseia-se no conceito de **Dependência Funcional**;
- Se `A → B`, então **B é funcionalmente dependente de A**;
- Armazenar B juntamente com A caracteriza **redundância funcional**.

---
## Exemplos Clássicos

- `data_nascimento → idade`
- `quantidade × valor_unitário → valor_total`
- `codigo_produto → descricao_produto`
- `cep → cidade, estado`

---
## Impactos

### Vantagens
- Possível ganho de desempenho;
- Simplificação de consultas;
- Redução de cálculos frequentes.

### Desvantagens
- Risco de inconsistência;
- Necessidade de controle de atualização;
- Aumento de complexidade de manutenção.

---
## Relação com Normalização

> [!important]
> A normalização **elimina a redundância funcional**, especialmente nas **formas normais (2FN, 3FN e BCNF)**, ao separar atributos funcionalmente dependentes.

---
## Redundância Funcional × Redundância Controlada

> [!tip]
> A redundância funcional **pode ser controlada**, desde que haja mecanismos adequados (triggers, regras de negócio).

---
## Tópicos Relacionados

- [[Dependência Funcional]]
- [[Normalização]]
- [[Redundância Controlada]]
- [[Redundância Não Controlada]]
- [[Anomalias de Dados]]
