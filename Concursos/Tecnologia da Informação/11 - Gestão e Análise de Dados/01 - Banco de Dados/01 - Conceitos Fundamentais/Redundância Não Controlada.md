---
disciplina: Tecnologia da Informação
tópico: Banco de Dados
created: 2026-01-06T16:30:00
updated: 2026-01-06T16:35:00
---

## Conceito

> [!note] Redundância Não Controlada
> Ocorre quando **a mesma informação é armazenada repetidamente** no banco de dados **sem planejamento ou mecanismos de controle**, geralmente em razão de **falhas de modelagem** e **ausência de normalização**.

#tecnologia_informacao/banco_dados/redundancia_nao_controlada

---
## Características

- Repetição desnecessária de dados;
- Falta de regras para sincronização;
- Alto risco de inconsistência;
- Estrutura de dados mal projetada.

---
## Principais Consequências (Anomalias)

- **Anomalia de Inserção**  
  → impossibilidade de inserir um dado sem outro relacionado.

- **Anomalia de Atualização**  
  → necessidade de alterar o mesmo dado em vários locais.

- **Anomalia de Exclusão**  
  → perda involuntária de informações relevantes.

---
## Causas Comuns

- Tabelas não normalizadas;
- Atributos multivalorados;
- Dependências funcionais incorretas;
- Violação das formas normais (1FN, 2FN, 3FN).

---
## Relação com Normalização

> [!important]
> A **normalização** tem como objetivo **eliminar a redundância não controlada**, preservando a integridade e a consistência dos dados.

---
## Tópicos Relacionados

- [[Normalização]]
- [[Anomalias de Dados]]
- [[Dependência Funcional]]
- [[Redundância Controlada]]
